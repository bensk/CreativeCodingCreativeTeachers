---
layout: "page"
title: "🔁 Loops"
---

## Do Now (in p5)
In p5, draw as many circles as you can in the next 3 minutes.

<iframe src="http://alpha.editor.p5js.org/embed/ByWSpbQQe" width = "100%" height = "300px;" style="border:none;"></iframe>

## Loopy
Drawing a bunch of circles is terrible. Let's not do that.

<script type="text/p5" data-autoplay data-preview-width="300" data-preview-height="">
function setup() {
  createCanvas(windowWidth, windowHeight);
}

function draw() {
  x = 50;
  while(x<windowWidth){
    ellipse(x,50,50,50);
    x = x + 50;
  }
}
</script>

`function draw()` is a loop. What if we wanted to write our own?

### One place I learn new things:

<iframe src="https://player.vimeo.com/video/139013336" width="640" height="360" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
<p><a href="https://vimeo.com/139013336">4.1 p5.js: while and for loop</a> from <a href="https://vimeo.com/shiffman">shiffman</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

## `while` loops

Work like a **conditional**:

```javascript
if (something True){
    // do this code
} else {
    // do this code
}
```

```js
while(something True){
    // run this code over and over again
}
```
