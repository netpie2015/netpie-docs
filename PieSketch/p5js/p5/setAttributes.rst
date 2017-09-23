.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

setAttributes()
===============

Set attributes for the WebGL Drawing context.
This is a way of adjusting ways that the WebGL
renderer works to fine-tune the display and performance.
This should be put in setup().
The available attributes are:

alpha - indicates if the canvas contains an alpha buffer
default is true

depth - indicates whether the drawing buffer has a depth buffer
of at least 16 bits - default is true

stencil - indicates whether the drawing buffer has a stencil buffer
of at least 8 bits

antialias - indicates whether or not to perform anti-aliasing
default is false

premultipliedAlpha - indicates that the page compositor will assume
the drawing buffer contains colors with pre-multiplied alpha
default is false

preserveDrawingBuffer - if true the buffers will not be cleared and
and will preserve their values until cleared or overwritten by author
(note that p5 clears automatically on draw loop)
default is true


<div>
<code>
 function setup() {
  createCanvas(150,150,WEBGL);
 }
 function draw() {
  background(255);
  push();
  rotateZ(frameCount * 0.02);
  rotateX(frameCount * 0.02);
  rotateY(frameCount * 0.02);
  fill(0,0,0);
  box(50);
  pop();
 }
</code>
</div>

Now with the antialias attribute set to true.

<div>
<code>
 function setup() {
  createCanvas(150,150,WEBGL);
  setAttributes('antialias', true);
 }
 function draw() {
  background(255);
  push();
  rotateZ(frameCount * 0.02);
  rotateX(frameCount * 0.02);
  rotateY(frameCount * 0.02);
  fill(0,0,0);
  box(50);
  pop();
 }
</code>
</div>

**รูปแบบการใช้งาน**

setAttributes ( String, New )

**พารามิเตอร์**

- ``String``  : name of attribute or object with key-value pairs

- ``New``  : value of named attribute


.. toctree::

