.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

draw()
======

Called directly after setup(), the draw() function continuously executes
the lines of code contained inside its block until the program is stopped
or noLoop() is called. Note if noLoop() is called in setup(), draw() will
still be executed once before stopping. draw() is called automatically and
should never be called explicitly.

It should always be controlled with noLoop(), redraw() and loop(). After
noLoop() stops the code in draw() from executing, redraw() causes the
code inside draw() to execute once, and loop() will cause the code
inside draw() to resume executing continuously.

The number of times draw() executes in each second may be controlled with
the frameRate() function.

There can only be one draw() function for each sketch, and draw() must
exist if you want the code to run continuously, or to process events such
as mousePressed(). Sometimes, you might have an empty call to draw() in
your program, as shown in the above example.

It is important to note that the drawing coordinate system will be reset
at the beginning of each draw() call. If any transformations are performed
within draw() (ex: scale, rotate, translate, their effects will be
undone at the beginning of draw(), so transformations will not accumulate
over time. On the other hand, styling applied (ex: fill, stroke, etc) will
remain in effect.

**รูปแบบการใช้งาน**

draw ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var yPos = 0;
	function setup() {  // setup() runs once
	  frameRate(30);
	}
	function draw() {  // draw() loops forever, until stopped
	  background(204);
	  yPos = yPos - 1;
	  if (yPos < 0) {
	    yPos = height;
	  }
	  line(0, yPos, width, yPos);
	}
	</script>

	<br><br>

.. toctree::

