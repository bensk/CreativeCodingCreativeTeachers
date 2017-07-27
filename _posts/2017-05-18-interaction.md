---
title: ↔️ Interaction
date: 2017-05-18 07:29:00 Z
layout: post
---

## Do Now (In Google Classroom)
What is a variable?    
How did we create variables in Python?    
How did we create variables in JavaScript?    
Why do we user variables in code?    

## Built-in Variables in <span style="color: #ED1F5E">p5</span>
We've actually seen a few variables in p5 already.

Look at the code below:

<script type="text/p5" data-autoplay data-preview-width="300" data-preview-height="">
// This goes at the top of your code
function setup(){
    createCanvas(windowWidth,windowHeight)
}

function draw(){
background('white')
textSize(10)
text('Mouse X = ' + mouseX + " | Mouse Y = " + mouseY, 10, 10)
}
</script>

What are `mouseX` and `mouseY` equal to? If you said "it keeps changing!" you're absolutely right. These are variables.

Take a closer look at my code. How **big** is my canvas? If you said "it keeps changing!" you...get the idea. Also variables.

### Exploring variables
✱ Create a canvas that is the width and height of the window.

✱ Draw a `line()` from the top middle of your screen (just below the camera) to your mouse cursor.

> Hint: you will need variables to create the canvas. How could use those same variables to find **half** your screen?

It should look something like this:

<script type="text/p5" data-autoplay data-preview-width="800" data-preview-height="">
function setup() {
  createCanvas(windowWidth,windowHeight)
}

function draw() {
  background('white')
  line(windowWidth/2,0,mouseX,mouseY)
}
</script>

> Extend yourself! Give the line a different `stroke` and `strokeWeight`    
>Are you seeing a whole bunch of lines? How can you draw _only one_?    
> Can you "hang" a rectangle off the end of the line?    

### Back to the ~~Drawing board~~ Canvas
Go back to either your snowman or your own drawing, and add variables. But sure to use:

- `windowWidth`
- `windowHeight`
- `mouseX`
- `mouseY`

## <span class="mega-octicon octicon-rocket"></span> Push yourself for a 4!
Can you make your `fill()` or `stroke()` as you move the mouse?
