# Grammatical Framework (GF) language grammar for highlight.js

## Usage

Simply include the Highlight.js library in your webpage or Node app, then load this module.

### Static website or simple usage

Simply load the module after loading Highlight.js.
You'll use the minified version found in the `dist` directory.
This module is just a CDN build of the language, so it will register itself as the Javascript is loaded.

```html
<script type="text/javascript" src="/path/to/highlight.min.js"></script>
<script type="text/javascript" src="/path/to/gf.min.js"></script>
<script type="text/javascript">
  hljs.initHighlightingOnLoad();
</script>
```

### Using directly from the UNPKG CDN

```html
<script type="text/javascript"
  src="https://unpkg.com/highlightjs-gf/dist/gf.min.js"></script>
```

- More info: <https://unpkg.com>

### With Node or another build system

If you're using Node / Webpack / Rollup / Browserify, etc, simply require the language module, then register it with Highlight.js.

```javascript
var hljs = require('highlightjs');
var hljsGF = require('highlightjs-gf');

hljs.registerLanguage("gf", hljsGF);
hljs.highlightAll();
```


## License

This package is released under the MIT License. See [LICENSE][1] file for details.

### Author/Maintainer

John J. Camilleri <john@johnjcamilleri.com>


## Links

- This package (and README) is closely based on Josh Goebel's [highlightjs-robots-txt](https://github.com/highlightjs/highlightjs-robots-txt)
- The official site for the Highlight.js library is <https://highlightjs.org/>.
- The Highlight.js GitHub project: <https://github.com/highlightjs/highlight.js>
- Learn more about Grammatical Framework: <https://www.grammaticalframework.org/>

[1]: https://github.com/johnjcamilleri/highlightjs-gf/blob/master/LICENSE
