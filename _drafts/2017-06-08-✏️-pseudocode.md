---
title: "✏️ Pseudocode"
date: 2017-06-08 16:06:00 Z
layout: post
---

## Do Now
Write down instructions to walk around the edge of the room.

## Mini Lesson
**Pseudocode** <sup>(noun)</sup> Simplified instructions that can be turned into code.

Remember the 🍞 PB&J?

Pseudocode will go in our `// comments` and are helpful for reminders from our past self to our future self.

Let's write out pseudocode for the four conditionals needed to make a path around the screen.

## Pseudocode Practice Make Pseudoperfect

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

## Our Notes

```js
// if y <= 32, x = x + 1
// if x >= windowWidth - 10, y = y + 1
// if y >= windowHeight - 32, x = x - 1
// if x <= 32, y = y - 1
```
