# js-promises

One way of using promises is calling `.then()` on a promise and passing it a "callback" function. The callback function tells a computer what to do when the promise has successfully returned some data. Your code might look something like this:

```javascript
functionReturingPromise().then(data => {
    doStuffWithData(data);
});
```

A real-life example of this is using fetch:

```javascript
fetch('https://random-data-api.com/api/users/random_user').then(response => {
    console.log(`The server successfully processed your request and responded with status code: ${ response.status }
    For serious information on status codes see: https://developer.mozilla.org/en-US/docs/Web/HTTP/Status
    For more interseting info see: https://http.cat/`);
});
```

When you're ready to dig into promises `git checkout step-02`