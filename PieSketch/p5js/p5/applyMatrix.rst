.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

applyMatrix()
=============

Multiplies the current matrix by the one specified through the parameters.
This is a powerful operation that can perform the equivalent of translate,
scale, shear and rotate all at once. You can learn more about transformation
matrices on <a href="https://en.wikipedia.org/wiki/Transformation_matrix">
Wikipedia</a>.
The naming of the arguments here follows the naming of the <a href=
"https://html.spec.whatwg.org/multipage/canvas.html#dom-context-2d-transform">
WHATWG specification</a> and corresponds to a
transformation matrix of the
form:
> <img style="max-width: 150px" src="assets/transformation-matrix.png"
alt="The transformation matrix used when applyMatrix is called"/>

**รูปแบบการใช้งาน**

applyMatrix ( a, b, c, d, e, f )

**พารามิเตอร์**

- ``a``  : numbers which define the 2x3 matrix to be multiplied

- ``b``  : numbers which define the 2x3 matrix to be multiplied

- ``c``  : numbers which define the 2x3 matrix to be multiplied

- ``d``  : numbers which define the 2x3 matrix to be multiplied

- ``e``  : numbers which define the 2x3 matrix to be multiplied

- ``f``  : numbers which define the 2x3 matrix to be multiplied


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  frameRate(10);
	  rectMode(CENTER);
	}
	
	function draw() {
	  var step = frameCount % 20;
	  background(200);
	  // Equivalent to translate(x, y);
	  applyMatrix(1, 0, 0, 1, 40 + step, 50);
	  rect(0, 0, 50, 50);
	}
	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  frameRate(10);
	  rectMode(CENTER);
	}
	
	function draw() {
	  var step = frameCount % 20;
	  background(200);
	  translate(50, 50);
	  // Equivalent to scale(x, y);
	  applyMatrix(1 / step, 0, 0, 1 / step, 0, 0);
	  rect(0, 0, 50, 50);
	}
	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  frameRate(10);
	  rectMode(CENTER);
	}
	
	function draw() {
	  var step = frameCount % 20
	  var angle = map(step, 0, 20, 0, TWO_PI);
	  var cos_a = cos(angle);
	  var sin_a = sin(angle);
	  background(200);
	  translate(50, 50);
	  // Equivalent to rotate(angle);
	  applyMatrix(cos_a, sin_a, -sin_a, cos_a, 0, 0);
	  rect(0, 0, 50, 50);
	}
	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  frameRate(10);
	  rectMode(CENTER);
	}
	
	function draw() {
	  var step = frameCount % 20
	  var angle = map(step, 0, 20, -PI/4, PI/4);
	  background(200);
	  translate(50, 50);
	  // equivalent to shearX(angle);
	  var shear_factor = 1 / tan(PI/2 - angle);
	  applyMatrix(1, 0, shear_factor, 1, 0, 0);
	  rect(0, 0, 50, 50);
	}
	</script>

	<br><br>

.. toctree::

