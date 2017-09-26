.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

min()
=====

กำหนดค่าที่เล็กที่สุดในลำดับของตัวเลขจากนั้นส่งคืนค่านั้น min () รับหมายเลขพารามิเตอร์จำนวนหนึ่งหรืออาร์เรย์ยาว ๆ

.. Determines the smallest value in a sequence of numbers, and then returns
.. that value. min() accepts any number of Number parameters, or an Array
.. of any length.

**รูปแบบการใช้งาน**

min ( n0 )

**พารามิเตอร์**

- ``n0``  Number,Array: ตัวเลขเพื่อเปรียบเทียบ

.. ``n0``  Number,Array: Numbers to compare

**ค่าที่ส่งออกมา**

- Number: จำนวนขั้นต่ำ

.. Number: minimum Number

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

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
