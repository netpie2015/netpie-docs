.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

norm()
======

Normalizes จำนวนจากช่วงอื่นเป็นค่าระหว่าง 0 และ 1 เหมือนกับแผนที่ (ค่า, ต่ำ, สูง, 0, 1) ตัวเลขนอกช่วงไม่ได้รับการติดตั้งเป็น 0 และ 1 เนื่องจากค่าที่อยู่นอกช่วงมีความตั้งใจและเป็นประโยชน์ (ดูตัวอย่างที่สองข้างต้น)

.. Normalizes a number from another range into a value between 0 and 1.
.. Identical to map(value, low, high, 0, 1).
.. Numbers outside of the range are not clamped to 0 and 1, because
.. out-of-range values are often intentional and useful. (See the second
.. example above.)

**รูปแบบการใช้งาน**

norm ( value, start, stop )

**พารามิเตอร์**

- ``value``  Number: ค่าขาเข้าที่จะเป็นปกติ

- ``start``  Number: ขอบเขตล่างของช่วงปัจจุบันของค่า

- ``stop``  Number: ขอบเขตบนของช่วงปัจจุบันของค่า

.. ``value``  Number: incoming value to be normalized
.. ``start``  Number: lower bound of the value's current range
.. ``stop``  Number: upper bound of the value's current range

**ค่าที่ส่งออกมา**

- Number: จำนวนปกติ

.. Number: normalized number

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

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
