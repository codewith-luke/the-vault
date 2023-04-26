https://developer.mozilla.org/en-US/docs/Web/API/Broadcast_Channel_API

This is used for communication between browing contexts (windows, tabs, frames, iframes) on the same origin.

#### Create channel

```js
const bc = new BroadcastChannel("test_channel");
```

#### Send Message

```js
bc.postMessage("This is a test message.");
```

#### Recieve Message

```js
bc.onmessage = (event) => {
  console.log(event);
};
```

#### Close Channel

```js
bc.close();
```