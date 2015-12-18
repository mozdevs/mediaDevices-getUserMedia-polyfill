# mediaDevices-getUserMedia-polyfill

> A polyfill to use the Promise-flavoured, `mediaDevices` based version of getUserMedia, in browsers that support *some sort* of getUserMedia.

With this polyfill you can access getUserMedia like this:

```javascript
navigator.mediaDevices.getUserMedia({ video: true, audio: true }).then(function(stream) {

}, function(error) {

});
```

versus the old version:

```javascript
navigator.getUserMedia({ video: true, audio: true }, function(stream) {

}, function(error) {

});
```

Look at [index.html](example/index.html) and [main.js](./example/main.js) in the [example](./example) folder to see how to use the result of the stream to display a video on screen when successful, or how to detect errors and showing a message to the user.

Here is a list of [browser support for WebRTC / getUserMedia](http://iswebrtcreadyyet.com/).
