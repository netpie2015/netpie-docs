.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

min()
=====

Determines the smallest value in a sequence of numbers, and then returns
that value. min() accepts any number of Number parameters, or an Array
of any length.

**รูปแบบการใช้งาน**

min ( n0 )

**พารามิเตอร์**

- ``n0``  : Numbers to compare


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  // Change the elements in the array and run the sketch
	  // to show how min() works!
	  numArray = new Array(2,1,5,4,8,9);
	  fill(0);
	  noStroke();
	  text("Array Elements", 0, 10);
	  // Draw all numbers in the array
	  var spacing = 15;
	  var elemsY = 25;
	  for(var i = 0; i < numArray.length; i++) {
	    text(numArray[i], i * spacing, elemsY);
	  }
	  maxX = 33;
	  maxY = 80;
	  // Draw the Minimum value in the array.
	  textSize(32);
	  text(min(numArray), maxX, maxY);
	}
	</script>

	<br><br>

.. toctree::

