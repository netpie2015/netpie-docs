.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

mag()
=====

Calculates the magnitude (or length) of a vector. A vector is a direction
in space commonly used in computer graphics and linear algebra. Because it
has no "start" position, the magnitude of a vector can be thought of as
the distance from the coordinate 0,0 to its x,y value. Therefore, mag() is
a shortcut for writing dist(0, 0, x, y).

**รูปแบบการใช้งาน**

mag ( a, b )

**พารามิเตอร์**

- ``a``  Number: first value

- ``b``  Number: second value


**ค่าที่ส่งออกมา**

- Number: magnitude of vector from (0,0) to (a,b)


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var x1 = 20;
	  var x2 = 80;
	  var y1 = 30;
	  var y2 = 70;
	
	  line(0, 0, x1, y1);
	  print(mag(x1, y1));  // Prints "36.05551275463989"
	  line(0, 0, x2, y1);
	  print(mag(x2, y1));  // Prints "85.44003745317531"
	  line(0, 0, x1, y2);
	  print(mag(x1, y2));  // Prints "72.80109889280519"
	  line(0, 0, x2, y2);
	  print(mag(x2, y2));  // Prints "106.3014581273465"
	}

	</script>

	<br><br>

.. toctree::

