.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

exp()
=====

Returns Euler's number e (2.71828...) raised to the power of the n
parameter. Maps to Math.exp().

**รูปแบบการใช้งาน**

exp ( n )

**พารามิเตอร์**

- ``n``  Number: exponent to raise


**ค่าที่ส่งออกมา**

- Number: e^n


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function draw() {
	  background(200);
	
	  // Compute the exp() function with a value between 0 and 2
	  var xValue = map(mouseX, 0, width, 0, 2);
	  var yValue = exp(xValue);
	
	  var y = map(yValue, 0, 8, height, 0);
	
	  var legend = "exp (" + nfc(xValue, 3) +")\n= " + nf(yValue, 1, 4);
	  stroke(150);
	  line(mouseX, y, mouseX, height);
	  fill(0);
	  text(legend, 5, 15);
	  noStroke();
	  ellipse (mouseX,y, 7, 7);
	
	  // Draw the exp(x) curve,
	  // over the domain of x from 0 to 2
	  noFill();
	  stroke(0);
	  beginShape();
	  for (var x = 0; x < width; x++) {
	    xValue = map(x, 0, width, 0, 2);
	    yValue = exp(xValue);
	    y = map(yValue, 0, 8, height, 0);
	    vertex(x, y);
	  }
	
	  endShape();
	  line(0, 0, 0, height);
	  line(0, height-1, width, height-1);
	}

	</script>

	<br><br>

.. toctree::

