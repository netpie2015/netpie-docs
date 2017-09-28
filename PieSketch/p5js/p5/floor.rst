.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

floor()
=======

คำนวณค่า int ที่ใกล้เคียงที่สุดที่น้อยกว่าหรือเท่ากับค่าของพารามิเตอร์ Maps to Math.floor ()

.. Calculates the closest int value that is less than or equal to the
.. value of the parameter. Maps to Math.floor().

**รูปแบบการใช้งาน**

floor ( n )

**พารามิเตอร์**

- ``n``  Number: จำนวนรอบ

.. ``n``  Number: number to round down

**ค่าที่ส่งออกมา**

- Number: ตัวเลขปัดเศษ

.. Number: rounded down number

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function draw() {
	  background(200);
	  //map, mouseX between 0 and 5.
	  var ax = map(mouseX, 0, 100, 0, 5);
	  var ay = 66;
	
	  //Get the floor of the mapped number.
	  var bx = floor(map(mouseX, 0, 100, 0,5));
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

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
