---
layout: "page"
title: "Roll the 🎲"
---

Let’s say we throw two dice on the ground. What number did we roll?

Press <span style="color: #ED1F5E">▶ Play</span> below.

<script type="text/p5" data-height="490" data-preview-width="470">
function setup() {
	createCanvas(windowWidth, windowHeight);
	background('#ED245E');
}

function draw() {
	strokeWeight(3);
	stroke('black');
	fill(255);
	rect(20, 20, 200, 200);
	fill('blue');
	ellipse(120, 120, 50, 50);
	fill(255);
	rect(250, 20, 200, 200);
	fill('blue');
	ellipse(300, 70, 50, 50);
	ellipse(350, 120, 50, 50);
	ellipse(400, 170, 50, 50);
}
</script>

Now it’s your turn. We need 6's to win! Modify the code to make each dice always show a 6.

## Roll the Die

1. Change the color of your die
2. Change the color of the background
3. Move the die around the screen
4. Add another die
