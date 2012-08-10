
# Progress

  Circular progress indicator using canvas.

  ![js progress indicator component](http://f.cl.ly/items/1i0B0D1i1D1Y1e1M1S08/Screen%20Shot%202012-08-10%20at%2011.48.22%20AM.png)

## Installation

```
$ npm install progress-component
```

## Example

```js
var Progress = require('progress');

var progress = new Progress;
document.body.appendChild(progress.render());

var n = 0;
var id = setInterval(function(){
  if (n == 100) clearInterval(id);
  progress.update(n++);
}, 50);
```

## API
  
### Progress#update(n)

  Update the indicator to `n` and re-draw.

### Progress#font(family)

  Change the font to `family`.

### Progress#fontSize(n)

  Change the font size to `n`.

### Progress#size(n)

  Change the indicator diameter to `n`, defaults to 50.

## License

  MIT