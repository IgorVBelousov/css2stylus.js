# css2stylus.js

JavaScript utility to convert CSS into Stylus.

Node/Browser compatible.

## Usage

### Node

Install the module
```bash
$ npm install -g css2stylus
```

Convert any css file:
```bash
$ css2stylus myfile.css
```

The output will be saved to `myfile.styl`.

### Browser

```html
<!doctype html>
  <title>Demo</title>
  <script src="css2stylus.js"></script>
  <script>
  (function () {
    var css = 'body { color: red; }';
    var converter = new Css2Stylus.Converter(css);
    converter.processCss();
    // output
    var stylus_output = converter.getStylus();
    // body
    //   color red
  }());
  </script>
```

## License
See [LICENSE.txt](https://raw.github.com/dciccale/css2stylus.js/master/LICENSE.txt)