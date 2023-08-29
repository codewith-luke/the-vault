##### Prerequisites
Before starting make sure that you have a basic understanding of: [TCP](https://www.khanacademy.org/computing/computers-and-internet/xcae6f4a7ff015e7d:the-internet/xcae6f4a7ff015e7d:transporting-packets/a/transmission-control-protocol--tcp) 
## How to
In Go we will make use of the [io.Reader](https://www.youtube.com/watch?v=O-MeKOuvzYE) interface. You can also checkout [io.Writer](https://www.youtube.com/watch?v=A1MS2LHcPuE). I found these videos useful for digesting how we will interact with TCP connections and buffers of data.

In a Go TCP Client => Server we need to deal with Buffers. I am going to give you all the information up front here and we will unpack it:

*client.go*
```go 
package main

import (
	"bufio"
	"fmt"
	"io"
	"net"
	"os"
	"time"
)

const (
	HOST = "localhost"
	PORT = "8080"
	TYPE = "tcp"
)

func main() {
	tcpServer, err := net.ResolveTCPAddr(TYPE, HOST+":"+PORT)

	if err != nil {
		println("ResolveTCPAddr failed:", err.Error())
		os.Exit(1)
	}

	conn, err := net.DialTCP(TYPE, nil, tcpServer)
	if err != nil {
		println("Dial failed:", err.Error())
		os.Exit(1)
	}

	_, err = conn.Write([]byte("This is a message\n"))
	if err != nil {
		println("Write data failed:", err.Error())
		os.Exit(1)
	}

	time.Sleep(5 * time.Second)
	_, err = conn.Write([]byte("This is a message 2\n test"))

	handleClient(conn)
	conn.Close()
}

func handleClient(conn net.Conn) {
	defer conn.Close()
	reader := bufio.NewReader(conn)

	buf := make([]byte, 1024)

	for {
		data, err := reader.Read(buf)

		if err == io.EOF {
			break
		}

		if err != nil {
			fmt.Println("Error reading:", err.Error())
			os.Exit(1)
		}

		fmt.Println("Received message:", string(buf[:data]))
	}
}
```

*server.go*
```go
package main

import (
	"bufio"
	"fmt"
	"io"
	"log"
	"net"
	"os"
)

const (
	HOST = "localhost"
	PORT = "8080"
	TYPE = "tcp"
)

func main() {
	listen, err := net.Listen(TYPE, HOST+":"+PORT)

	if err != nil {
		log.Fatal(err)
	}

	defer listen.Close()

	for {
		conn, err := listen.Accept()
		if err != nil {
			log.Fatal(err)
			os.Exit(1)
		}
		go handleServer(conn)
	}
}

func handleServer(conn net.Conn) {
	defer conn.Close()
	reader := bufio.NewReader(conn)

	for {
		data, err := reader.ReadString('\n')
		fmt.Println("reading data")
		if err == io.EOF {
			fmt.Println("EOF")
			break
		}

		if err != nil {
			fmt.Println("Error reading:", err.Error())
			os.Exit(1)
		}

		fmt.Println("Received message:", string(data))
		break
	}

	fmt.Println("writing response")
	conn.Write([]byte("Message received.\n"))
}
```

In the above we have setup a basic server and client that communicate over TCP. I am going to gloss over the main function for the *server.go*. In Short it sets up a persistent server that listens for connections.

The important part to grasp here is the *handleServer* ,*handleClient* methods.

Each of these execpts a *net.Conn*. When a connection is established from client to the server this connection stays open until we *conn.Close()* from either end.

What both of these methods do is create a new *bufio* reader with that open connection and then create a loop that reads from that buffer.

```go
func handleServer(conn net.Conn) {
	defer conn.Close()
	reader := bufio.NewReader(conn)

	for {
		data, err := reader.ReadString('\n')
		fmt.Println("reading data")
		if err == io.EOF {
			fmt.Println("EOF")
			break
		}

		if err != nil {
			fmt.Println("Error reading:", err.Error())
			os.Exit(1)
		}

		fmt.Println("Received message:", string(data))
		break
	}

	fmt.Println("writing response")
	conn.Write([]byte("Message received.\n"))
}
```

We can just look at this *handleServer* to understand how both will work. This for loop will stay open till either a `io.EOF` error, error or until it reads its first message successfully.

`reader.Readstring` will read from the open connection buffer and will write to a data variable which we will then print out, proceed to break out of the loop and then write a response back to the client.

So what would it read?

```go
_, err = conn.Write([]byte("This is a message\n"))
	if err != nil {
		println("Write data failed:", err.Error())
		os.Exit(1)
	}

time.Sleep(5 * time.Second)
_, err = conn.Write([]byte("This is a message 2\n test"))
```

In our client we send a message `This is a message`. The server will log that out and return a response `conn.Write`. However you may notice that we will wait 5s and send another message. You may also notice that you won't see the second message on the server and won't see the response until such time that on the client we make use of `handleClient`.

The reason for this is due to the following flow:

1) We create a connection
2) We send a packet of data (string)
3) We read that packet using a bufio reader
4) It breaks out of the reader, meaning we no longer are reading from the stream
5) We send a response
6) It then sends another packet after 5s
7) It then handles any data sent back from the server

If you had to remove the break from the server loop. It will then never send a response. Because we need to give it an exit strategy. In other words, we need the client to tell the server it is done sending data and it can now close.

The alternative is you can send a response for every packet and this will handle as well.

## Encoding/Decoding Data







If you have two servers that are written in Go it might be a good use case for checking out [[Gobs]].