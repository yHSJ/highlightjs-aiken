# highlightjs-aiken
Aiken is a smart contract platform for Cardano.

## Usage
Include the `highlight.js` library in your project and then load this module.

### Static Website
If you are using a static website, simply load the module after loading `highlight.js`.
```html
<script type="text/javascript" src="/path/to/highlight.min.js"></script>
<script type="text/javascript" src="/path/to/aiken.min.js"></script>
<script type="text/javascript">
  hljs.highlightAll();
</script>
```

### Node or other build system
If you're using Node or another build system, you can require the language module, then reigster it with `highlight.js`
```javascript
var hljs = require('highlight.js');
var hljsAikenTxt = require('highlightjs-aiken');

hljs.registerLanguage("aiken", hljsAikenTxt);
hljs.highlightAll();
````
