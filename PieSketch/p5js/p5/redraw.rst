.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

redraw()
========

Executes the code within draw() one time. This functions allows the
program to update the display window only when necessary, for example
when an event registered by mousePressed() or keyPressed() occurs.

In structuring a program, it only makes sense to call redraw() within
events such as mousePressed(). This is because redraw() does not run
draw() immediately (it only sets a flag that indicates an update is
needed).

The redraw() function does not work properly when called inside draw().
To enable/disable animations, use loop() and noLoop().

In addition you can set the number of redraws per method call. Just
add an integer as single parameter for the number of redraws.

**รูปแบบการใช้งาน**

redraw ( [n] )

**พารามิเตอร์**

- ``n``  Integer: Redraw for n-times. The default value is 1.


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var x = 0;
	
	function setup() {
	  createCanvas(100, 100);
	  noLoop();
	}
	
	function draw() {
	  background(204);
	  line(x, 0, x, height);
	}
	
	function mousePressed() {
	  x += 1;
	  redraw();
	}
	var x = 0;
	
	function setup() {
	  createCanvas(100, 100);
	  noLoop();
	}
	
	function draw() {
	  background(204);
	  x += 1;
	  line(x, 0, x, height);
	}
	
	function mousePressed() {
	  redraw(5);
	}


	</script>

	<br><br>

.. toctree::

