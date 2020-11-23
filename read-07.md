# Read 07

## REST API

REST (Representational state transfer) is a software architectural style that defines a set of constraints to be used for creating Web services. Web services that conform to the REST architectural style, called RESTful Web services, provide interoperability between computer systems on the internet. The whole world wide web is built on an architectural style called “REST”. REST provides a definition of a “resource”, which is what those things point to.

## SuperAgent

SuperAgent is light-weight progressive ajax API crafted for flexibility, readability, and a low learning curve after being frustrated with many of the existing request APIs. It also works with Node.js.

SuperAgent has two implementations: one for web browsers (using XHR) and one for Node.JS (using core http module). By default Browserify and WebPack will pick the browser version.

Request basics:

```js
 request
   .get('/search')
   .then(res => {
      // res.body, res.headers, res.status
   })
   .catch(err => {
      // err.message, err.response
   });
```

Error handling:

```js
request.get('/404')
  .ok(res => res.status < 500)
  .then(response => {
    // reads 404 page as a successful response
  })
```

Forcing specific connection IP address:

```js
const res = await request.get("http://example.com").connect("127.0.0.1");
```

[Back to Home](README.md)
