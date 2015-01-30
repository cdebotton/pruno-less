# pruno-less

A LESS mix for pruno that includes font-awesome, normalize.css.

## Usage

```js
"use strict";

var pruno = require('pruno');

pruno.plugins(function(mix) {
  mix
    .configure({ dir: __dirname + '/config' })
    .less({
      'entry': '::src/less/index.less',
      'dist': '::dist/stylesheets/app.css',
      'search': '::src/**/*.less',
      'minify': false,
      'source-maps':true,
      'font-awesome': false,
      'normalize': false
    });
});
```
