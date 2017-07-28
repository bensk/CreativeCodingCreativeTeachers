---
title: "🤖 Motion"
layout: page
---

## Do Now
Create a sketch with an emoji that bounces off the edges of the screen.

> Hint: How do we make `text` in <span style="color: #ED1F5E">p5</span>? How did you make a shape "bounce" off the edge of the screen?

## Path around the edge
Very soon, we're going to build an interactive game in <span style="color: #ED1F5E">p5</span>, which will require us to be **very** good at using conditionals.

Now, instead of *reversing* direction when something hits the edge, we're going to make something follow a path *around* the edges of the screen.


## Pseudocode Practice Make Pseudoperfect

Pseudocode will go in our `// comments` and are helpful for reminders from our past self to our future self.

Let's write out pseudocode for the four conditionals needed to make a path around the screen.

![]({{ site.baseurl }}/images/pathAroundEdges.png)

Pretend you're talking to the emoji:

> "Go to the right until you hit the edge of the screen"

etc...

Now, we're going to see if we can be more specific in our pseudocode, by starting to add variables.

In your code, you will have some variables for the `x` and `y` position of the emoji. You also have the built-in variables of `windowWidth` and `windowHeight` to know where the edges of the screen are.

Underneath you pseudocode, write comments for how to go from pseudocode to <span style="color: #ED1F5E">p5</span> code.

| "Go to the right until you hit the edge of the screen"                                                                                      |
|:--------------------------------------------------------------------------------------------------------------------------------------------|
| // <code>y</code> stays close to top ( something like <code>y<=25</code>), <code>x</code> should move to the right (<code>x = x + 1</code>) |

## OM DOM DOM
We can use <span style="color: #ED1F5E">p5</span> to add familiar HTML elements to our sketches.

Try this out:

```js
var x
var y
var speed
var slider;

function setup() {
  createCanvas(windowWidth, windowHeight)
  x = windowWidth/2
  y = 30
  speed = 3
    // create a slider we can drag, from -30 to 30 and starting at 0
  slider = createSlider(-30, 30, 0);
  // set the position of the slider on the screen
  slider.position(windowWidth / 2-90, 90);
  // set the size of the slider
  slider.style('width', '180px');
}

function draw() {
  // We need to make a variable for the slider's value...
  var speed = slider.value();
  background('white')
  textSize(32)
  text("🤖", x, y)
  // ... so that we can move the robot
  x = x + speed
}
```

Now, add conditionals so that the robot (or emoji of your choice) follows a path around the screen, like this:

<iframe src="{{ site.baseurl }}/Code_Examples/PathAlongEdges" width="100%" height="400px" style="border:solid 1px; border-color: #ED1F5E"></iframe>

## Checklist

| Specification                                   | Points |
|:------------------------------------------------|:------:|
| An emoji, with a `textSize` of at least 24px    |   1    |
| At least 4 conditionals                         |   1    |
| Emoji follows path around screen                |   1    |
| Code functions correctly if window size changes |   1    |
| **Total**                                       |  __/4  |
| Extensions                                      | Points |
| Speed is adjustable                             |   1    |
| Use slider to adjust speed                      |   1    |
