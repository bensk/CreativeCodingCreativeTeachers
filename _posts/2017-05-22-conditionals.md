---
layout: "post"
title: "🚦Conditionals"
date: "2017-05-22 12:14"
---

## Do Now
1. Make an `ellipse()` that **follows** your mouse.
2. **After** your `ellipse()`, add this line:

```javascript
if (mouseX > 100) {
    text("what just happened?", 200, 200)
}
```

What happened? Why do you think that's happening?

## Conditionals
Conditionals in p5 work exactly like JavaScript conditionals. Thanks to our [built-in variables](http://bsk.education/CreativeCodingCreativeTeachers/2017/05/18/interaction/), we can quickly make sketches that **change** depending on where our mouse is.


## I'm on one side...
1. Create a canvas that is the size of the screen
2. Create a shape (`ellipse()`, `rect()`, etc) that follows your mouse
3. Write a conditional so that the `fill()` of the shape changes if the mouse is on the **left** or **right** side of the screen.

Like this:

<iframe src="{{ site.baseurl }}/Code_Examples/left_right/index.html" width="100%" height="200px" style="border:none"></iframe>

---

## Traffic Light

Create this "traffic light" in p5:

<iframe src="{{ site.baseurl }}/Code_Examples/TrafficLight" width="100%" height="400px" style="border:solid 1px"></iframe>

**Rubric**

| Specification                                                             | Points |
|:--------------------------------------------------------------------------|:------:|
| 3 ellipses, each light up different colors                                |   3    |
| It must be able to "light" up in three different colors **one at a time** |   1    |
| Only one light should be lit at a time                                    |   1    |
| Lights are **conditionally** activated[^1]                                |   1    |
| **Total**                                                                 |   6    |
