.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

ceil()
======

คำนวณค่า int ที่ใกล้เคียงซึ่งมากกว่าหรือเท่ากับค่าของพารามิเตอร์ Maps ไปยัง Math.ceil () ตัวอย่างเช่น ceil (9.03) ส่งกลับค่า 10

.. Calculates the closest int value that is greater than or equal to the
.. value of the parameter. Maps to Math.ceil(). For example, ceil(9.03)
.. returns the value 10.

**รูปแบบการใช้งาน**

ceil ( n )

**พารามิเตอร์**

- ``n``  Number: จำนวนรอบ

.. ``n``  Number: number to round up

**ค่าที่ส่งออกมา**

- Number: ปัดเศษขึ้นจำนวน

.. Number: rounded up number

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function draw() {
	  background(200);
	  // map, mouseX between 0 and 5.
	  var ax = map(mouseX, 0, 100, 0, 5);
	  var ay = 66;
	
	  //Get the ceiling of the mapped number.
	  var bx = ceil(map(mouseX, 0, 100, 0,5));
	  var by = 33;
	
	  // Multiply the mapped numbers by 20 to more easily
	  // see the changes.
	  stroke(0);
	  fill(0);
	  line(0, ay, ax * 20, ay);
	  line(0, by, bx * 20, by);
	
	  // Reformat the float returned by map and draw it.
	  noStroke();
	  text(nfc(ax, 2,2), ax, ay - 5);
	  text(nfc(bx,1,1), bx, by - 5);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
