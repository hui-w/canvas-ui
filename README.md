# Interactive Canvas
Javascript library for component-based HTML5 canvas

## A Brief Look

```js
// Create a canvas with border
var canvas = new Canvas(500, 100);
canvas.setProp('lineWidth', 1);

// Create a label
var label = new Label(10, 60, 0, 0, 'Label');

// Create a button and set its event handler
var button = new Button(10, 10, 130, 32, 'Click this button');
button.onTap.add(function(left, top) {
  var message = 'Button has been clicked at [' + left + ', ' + top + ']';
  label.setProp('text', message);
});

// Add controls into the canvas
canvas.controls.add(button);
canvas.controls.add(label);

// Render the canvas when everything is ready
var wrapper = $('brief-look-wrapper');
canvas.renderInto(wrapper);
```

## Components Overview
![image](https://raw.githubusercontent.com/hui-w/interactive-canvas/master/docs/overview.png)

## More Demo
https://hui-w.github.io/interactive-canvas

## API Reference
https://hui-w.github.io/interactive-canvas/reference.html
