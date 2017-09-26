.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

constrain()
===========

จำกัด ค่าระหว่างค่าต่ำสุดและสูงสุด

.. Constrains a value between a minimum and maximum value.

**รูปแบบการใช้งาน**

constrain ( n, low, high )

**พารามิเตอร์**

- ``n``  Number: จำนวนที่ จำกัด

- ``low``  Number: ขีด จำกัด ขั้นต่ำ

- ``high``  Number: ขีด จำกัด สูงสุด

.. ``n``  Number: number to constrain
.. ``low``  Number: minimum limit
.. ``high``  Number: maximum limit

**ค่าที่ส่งออกมา**

- Number: จำนวนข้อ จำกัด

.. Number: constrained number

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function draw() {
	  background(200);
	
	  var leftWall = 25;
	  var rightWall = 75;
	
	  // xm is just the mouseX, while
	  // xc is the mouseX, but constrained
	  // between the leftWall and rightWall!
	  var xm = mouseX;
	  var xc = constrain(mouseX, leftWall, rightWall);
	
	  // Draw the walls.
	  stroke(150);
	  line(leftWall, 0, leftWall, height);
	  line(rightWall, 0, rightWall, height);
	
	  // Draw xm and xc as circles.
	  noStroke();
	  fill(150);
	  ellipse(xm, 33, 9,9); // Not Constrained
	  fill(0);
	  ellipse(xc, 66, 9,9); // Constrained
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
