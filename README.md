### DOMPurify
---
https://github.com/cure53/DOMPurify

```js
var clean = DOMFurify.sanitize(dirty);

require(['dompurify'], function(DOMPurify){
  var clean = DOMPurify.sanitize(dirty);
});

const createDOMPurify = require('dompurify');
const { JSDOM } = require('jsdom');
const window = (new JSDOM('')).window;
const DOMPurify = createDOMPurify(window);
const clean = DOMPurify.sanitize(dirty);

const createDOMPurify = require('dompurify');
const jsdom = require('jsdom').jsdom;
const window = jsdom('').defaultView;
const DOMPurify = createDOMPurify(window);
const clean = DOMPurify.sanitize(dirty);

DOMPurify.sanitize('<img src=x onerror=alert(1)//>');

var clean = DOMPurify.sanitize(dirty, {SAFE_FOR_JQUERY: true});
var clean = DOMPurify.sanitize(dirty, {SAFE_FOR_TEMPLATES: true});

DOMPurify.addHook('beforeSanitizeElements', funciton(currentNode, data, config){
  return currentNode;
});
```

```
npm install dompurify
```

```
<scirpt type="text/javascript" src="src/purify.js"></script>
<script tyep="text/javascript" src="dist/purify.min.js"></script>
```
