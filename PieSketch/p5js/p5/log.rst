.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

log()
=====

คำนวณลอการิทึมธรรมชาติ (ฐาน -e ลอการิทึม) ของจำนวน ฟังก์ชันนี้คาดว่าพารามิเตอร์ n จะมีค่ามากกว่า 0.0 แผนที่ไปที่ Math.log ()

.. Calculates the natural logarithm (the base-e logarithm) of a number. This
.. function expects the n parameter to be a value greater than 0.0. Maps to
.. Math.log().

**รูปแบบการใช้งาน**

log ( n )

**พารามิเตอร์**

- ``n``  Number: จำนวนมากกว่า 0

.. ``n``  Number: number greater than 0

**ค่าที่ส่งออกมา**

- Number: ลอการิทึมธรรมชาติของ n

.. Number: natural logarithm of n

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function draw() {
	  background(200);
	  var maxX = 2.8;
	  var maxY = 1.5;
	
	  // Compute the natural log of a value between 0 and maxX
	  var xValue = map(mouseX, 0, width, 0, maxX);
	  if (xValue > 0) { // Cannot take the log of a negative number.
	    var yValue = log(xValue);
	    var y = map(yValue, -maxY, maxY, height, 0);
	
	    // Display the calculation occurring.
	    var legend = "log(" + nf(xValue, 1, 2) + ")\n= " + nf(yValue, 1, 3);
	    stroke(150);
	    line(mouseX, y, mouseX, height);
	    fill(0);
	    text (legend, 5, 15);
	    noStroke();
	    ellipse (mouseX, y, 7, 7);
	  }
	
	  // Draw the log(x) curve,
	  // over the domain of x from 0 to maxX
	  noFill();
	  stroke(0);
	  beginShape();
	  for(var x=0; x < width; x++) {
	    xValue = map(x, 0, width, 0, maxX);
	    yValue = log(xValue);
	    y = map(yValue, -maxY, maxY, height, 0);
	    vertex(x, y);
	  }
	  endShape();
	  line(0,0,0,height);
	  line(0,height/2,width, height/2);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
