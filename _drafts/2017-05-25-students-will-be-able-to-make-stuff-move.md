---
title: SWBAT Make Stuff Move
date: 2017-05-25 20:40:00 Z
layout: post
---

## Do Now (In Google Classroom)

Check this out:

<iframe src = "{{ site.baseurl}}/Code_Examples/MakeStuffMove/index.html" width ="100%" height="200px" style="border:none"></iframe>

Look at the code:

```javascript
function setup() {
    createCanvas(windowWidth, windowHeight)
    x = windowWidth / 2
    y = windowHeight / 2
}

function draw() {
    background('white')
    ellipse(x, y, 50, 50)

    x = x + 10
    if (x>windowWidth){
        x = 0
    }
}
```

1. Observe and describe the motion of the ellipse.
2. Which line do you think makes the ellipse move? Why?
3. Which line(s) do you think makes the ellipse start on the left side of the screen? Why?

---

## Incrementing Variables
If we were in math class, and I wrote: `x = x + 1`, what would you say?     

> "To solve `x = x + 1` subtract `x` from both sides, and you get `0=1`, which...makes no sense."

You would be right. Good thing we're not in math class.

<p class = "lead">In computer programming, <b>we can say <code>x = x+1</code></b>, and not only are we <b>correct</b>, it has a special name: <b>incrementing</b> a variable. </p>

In the Do Now, our initial `x` value was `x = windowWidth / 2` and our initial `y` value was `y = windowHeight / 2`. This put our `ellipse` at the center of the screen. The we ran:

```javascript
x = x + 10 // What happens to the x position?
```



## Back to Balls

| Specification                                                                          | Points |
|:---------------------------------------------------------------------------------------|:------:|
| Your `canvas` must resize to the window.                                               |   1    |
| User created variables for `x position`, `y position`, `x direction` and `y direction` |   3    |
| Conditionals for the left/right and top/bottom edge of the screen                      |   1    |
| **Extension**                                                                          |   ✱    |
| Ball bounces using only **2** conditionals                                             |   2    |
| **Total:**                                                                             | __ / 5 |



## Exit Slip
Complete the following sentences:    

> We increment variables because...    
> We increment variables but...    
> We increment variables so...    
