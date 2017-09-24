.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

lerp()
======

Calculates a number between two numbers at a specific increment. The amt
parameter is the amount to interpolate between the two values where 0.0
equal to the first point, 0.1 is very near the first point, 0.5 is
half-way in between, etc. The lerp function is convenient for creating
motion along a straight path and for drawing dotted lines.

**รูปแบบการใช้งาน**

lerp ( start, stop, amt )

**พารามิเตอร์**

- ``start``  Number: first value

- ``stop``  Number: second value

- ``amt``  Number: number between 0.0 and 1.0


**ค่าที่ส่งออกมา**

- Number: lerped value


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  background(200);
	  var a = 20;
	  var b = 80;
	  var c = lerp(a,b, .2);
	  var d = lerp(a,b, .5);
	  var e = lerp(a,b, .8);
	
	  var y = 50
	
	  strokeWeight(5);
	  stroke(0); // Draw the original points in black
	  point(a, y);
	  point(b, y);
	
	  stroke(100); // Draw the lerp points in gray
	  point(c, y);
	  point(d, y);
	  point(e, y);
	}


	</script>

	<br><br>

.. toctree::

