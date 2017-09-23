.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

norm()
======

Normalizes a number from another range into a value between 0 and 1.
Identical to map(value, low, high, 0, 1).
Numbers outside of the range are not clamped to 0 and 1, because
out-of-range values are often intentional and useful. (See the second
example above.)

**รูปแบบการใช้งาน**

norm ( value, start, stop )

**พารามิเตอร์**

- ``value``  : incoming value to be normalized

- ``start``  : lower bound of the value's current range

- ``stop``  : upper bound of the value's current range


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function draw() {
	  background(200);
	  currentNum = mouseX;
	  lowerBound = 0;
	  upperBound = width; //100;
	  normalized = norm(currentNum, lowerBound, upperBound);
	  lineY = 70
	  line(0, lineY, width, lineY);
	  //Draw an ellipse mapped to the non-normalized value.
	  noStroke();
	  fill(50)
	  var s = 7; // ellipse size
	  ellipse(currentNum, lineY, s, s);
	
	  // Draw the guide
	  guideY = lineY + 15;
	  text("0", 0, guideY);
	  textAlign(RIGHT);
	  text("100", width, guideY);
	
	  // Draw the normalized value
	  textAlign(LEFT);
	  fill(0);
	  textSize(32);
	  normalY = 40;
	  normalX = 20;
	  text(normalized, normalX, normalY);
	}
	</script>

	<br><br>

.. toctree::

