When running CPU intensive tasks it may be better to defer those tasks to an external process rather than blocking the the event loop.

So instead of blocking the main application we would instead use a separate process. This has a number of advantages:

1. The main I/O task can run at full speed.
2. Working with processes in Node is simple than let's say using something like setImmediate to get around the event loop.
3. If we need max performance the external process could be a lower level language.

```javascript
// parent.js
const { fork } = require('child_process');

// Create a child process by forking the child script
const childProcess = fork('child_script.js');

// Listen for messages from the child process
childProcess.on('message', (message) => {
  if (message === 'ready') {
    // Send a message to the child process
    childProcess.send('Hello from parent!');
  } else {
    console.log(`Message from child process: ${message}`);
  }
});

// Listen for the 'exit' event to know when the child process has exited
childProcess.on('exit', (code) => {
  console.log(`Child process exited with code ${code}`);
});
```

```javascript
// child_script.js

// Perform some time-consuming computation
function performComputation() {
	let result = 0;
	for (let i = 0; i < 1000000000; i++) {
	  result += i;
	}
	return result;
}


// Listen for messages from the parent process
process.on('message', (message) => {
  console.log(`Message from parent process: ${message}`);
  
  // Invoke the computation function
  const computationResult = performComputation();

  // Send the result back to the parent process
  process.send(`Computation result: ${computationResult}`);
});

process.send('ready');
```

The above shows a simple example of a child process that would perform some form of long running task. In this child process we are able to send messages back and forth in order to relay the status of what is going on.

This allows us to properly manager our child process and opens us up to being able to do things like pooling our processes as to not have to start them up later. Or to gracefully shut them down on issues.


