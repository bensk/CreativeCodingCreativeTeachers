---
layout: "page"
title: "ℹ️ Inputs"

---

## Do Now
What kinds of inputs are there on a web page?

## p5 Inputs
p5 makes inputs easy to create. We're going to use them to enhance our drawing app.

### `createInput()`

In our `setup()` function, we can create HTML elements, including input fields and sliders:

```js
input = createInput("✨");
// variable name = createInput("default value")
input.position(0, windowHeight);
```

### `createSlider()`

```js
slider = createSlider(32, width, 32);
// variable name = createSlider(min, max, starting value)
slider.position(0, windowHeight+20)
```

Once we have inputs, we want to pass those values into our `draw()` loop:

```js
var emoji = input.value();
var number = slider.value();
```

If I'm using the same variables in `setup()` and `draw()`, where should I be **declaring** those variables?

<iframe src="http://alpha.editor.p5js.org/embed/HJrGHRCWZ" frameborder="0" width = "100%"></iframe>

### Drawing App v2.0
Add **inputs** and **sliders** to control your drawing app. Be creative! What can you control with each kind of input?
