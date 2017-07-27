
<!-- layout: "page" -->
title: "Crazy Framerate"


<script type="text/p5" data-preview-width="400">   
function setup() {
  createCanvas(windowWidth,windowHeight);

}

function draw() {
  background('white');
  frameRate(log(mouseX)*5);
  var x = random(255);
  var y = random(255);
  var z = random(255);
  fill(x,y,z);

  rect(50,50,windowWidth-100,100,5);
  println(mouseX)
  textSize(36);
text("The framerate is " + log(mouseX)*9.2, 50, 30);

}

function windowResized() {
  resizeCanvas(windowWidth, windowHeight);
}
</script>

So, this might hurt your eyes.
