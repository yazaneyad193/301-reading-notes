# Read 11

## Embedded JavaScript templating (EJS)

 EJS is a simple templating language that lets you generate HTML markup with plain JavaScript. No religiousness about how to organize things. No reinvention of iteration and control-flow. It's just plain JavaScript.

Features of EJS:

* Fast compilation and rendering.
* Simple template tags: `<% %>`.
* Custom delimiters (e.g., use `[? ?]` instead of `<% %>`).
* Sub-template includes.
* Ships with CLI.
* Both server JS and browser support.
* Static caching of intermediate JavaScript.
* Static caching of templates.
* Complies with the Express view system.

EJS lets us spin up quick applications when we don’t need anything too complex. By using partials and having the ability to easily pass variables to our views, we can build some great applications quickly.

EJS can be installed using npm:

```shell
$ npm install ejs
```

Example on EJS:

```js
let ejs = require('ejs');
let people = ['geddy', 'neil', 'alex'];
let html = ejs.render('<%= people.join(", "); %>', {people: people});
```

[Back to Home](README.md)
