### Notes
- [Stream Examples](https://github.com/PacktPublishing/Node.js-Design-Patterns-Third-Edition/tree/master/06-coding-with-streams)
- See page `168` on Initialization Vector and Encryption

# Anatomy of Streams

There are 4 abstract classes available in the stream core module:

- Readable
- Writable
- Duplex
- Transform

One reason streams are so flexible is that it is not just binary data. They support 2 operating modes:

- Binary
- Object

## Readable Streams

When it comes to reading from a stream there are 2 modes:

- Flowing (or paused)
- Non-flowing

Non-flowing is the default and involves attaching a listener to the stream for the `readable` event whereas flowing mode is a little less flexible and data is pushed to the `data` listener as soon as it arrives.

### Read from iterables

It is also possible to read streams from iterables like an array. This can be achieved by using `Readable.from`

```ts
const mountaints = ['Everest', 'K2'];

const mountainStream = Readable.from(mountains);
```


## Backpressure

"Backpressure is similar to liquid flowing in a real pipe system"

This means streams can suffer from bottlenecks as well. This happens when data is written faster than the stream can consume it. The solution to this is buffering the incoming data. 

Problem is if the stream doesn't give feedback to the write where we have further backup.
This is preventable, `writeable.write()` will return false when the internal buffer exceed the `highWaterMark` limit. This is set in writeable streams as the limit of the internal buffer size. Anything higher it will start returning false.

When the buffer is emptied the `drain` event is emitted, which means it would be safe to write again. This is known as `backpressure`.

## Duplex Streams

Simply put this is a stream that is readable and writeable. This is useful when we want  to describe and entity that is both a data source and a destination such as `network sockets`. 

Similar to read/write streams we can determine the object mode. What is super powerful is that we can change the `readableObjectMode` and `writeableObjectMode` independently. Meaning one could use binary mode and the other could use object.

In a simple Duplex stream there is no immediate relationship between the data read from the stream and the data written into it (Think of a TCP socket, it is not aware of the relationship between the input and output).

## Transform Streams

Transform streams are a special kind of `Duplex` stream. They are designed to handle data transformations. 

When creating a Transform stream you would have your implementations of the `transform` and `flush` methods. 


