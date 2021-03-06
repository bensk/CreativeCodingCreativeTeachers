---
layout: "page"
title: "👆 Buttons & Functions"
---


## Try it
We created inputs with `createInput()` and sliders with `createSlider()`.

How do you think we can create a button?

## Buttons

<iframe src="http://alpha.editor.p5js.org/embed/SJeGmKHVl" width = "400" height = "300" style ="border:none"></iframe>


```js
var button;
function setup() {
  createCanvas(400, 300);
  button = createButton("Hello");
  button.position(width/2,height/2);
  background(50);
}
function draw() {
}
```

Ok that was easy. But a button is different than a slider or an input box. You don't get a value (string or integer). What do you get?

A click, or not a click. In terms of JavaScript, we call that an **event**.

# 🗓 Events
Whoa! We made a button. But clicking the button doesn’t **do** anything. To connect **clicking** a button to **doing** something, we need to define a function that contains the code that we want to run when the user clicks the button, and then attach an “event listener” to the object, to tell p5.js to call that particular function when the user takes a particular action. Luckily, half that work is done for us:

```js
var button;
function setup() {
  createCanvas(400, 300);
  button = createButton("Click me!");
  button.mousePressed(randomRectangle);
  background(50);
  noStroke();
}

```

This code uses the `.mousePressed()` event of the button object to call the function `randomRectangle()` when the user clicks a button.

Have you ever heard of the `randomRectangle()` function?

## BYOF

You haven't heard of it, because it's never existed before!

In p5, we have two built-in functions: `setup()` and `draw()`. So far, that's been enough. Not anymore!

```js
function randomRectangle() {
    fill(random(255));
    rect(random()*width, random()*height,
      random(400), random(400));
}
```

What's the name of this function? What does it do? When is it called?

## Clicker Game
You're going to make a terrible game, where every time the user click on a button, the button moves.

Create a canvas with a button located _somewhere_ to start. Then, define a function called `randomLocation()`  that will move the button around the screen when clicked.

## Pseudocode Checklist

✅ **How many variables do we need?**    
- What's changing? Declare each of those at the top of your code.

✅ **Create a button**    
- `button= createButton("Click or something...")`

✅ **Add an event to the button**    
- `button.mousePressed(randomLocation)`

✅ **Create the `randomLocation()` function**    
- Which of your variables should change to give a random location.
