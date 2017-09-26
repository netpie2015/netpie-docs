.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

round()
=======

คำนวณจำนวนเต็มใกล้เคียงกับพารามิเตอร์ n มากที่สุด ตัวอย่างเช่นรอบ (133.8) ส่งกลับค่า 134 แผนที่ไป Math.round ()

.. Calculates the integer closest to the n parameter. For example,
.. round(133.8) returns the value 134. Maps to Math.round().
**รูปแบบการใช้งาน**

round ( n )

**พารามิเตอร์**

- ``n``  Number: จำนวนรอบ

.. ``n``  Number: number to round

**ค่าที่ส่งออกมา**

- Number: เลขกลม

.. Number: rounded number

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function draw() {
	  background(200);
	  //map, mouseX between 0 and 5.
	  var ax = map(mouseX, 0, 100, 0, 5);
	  var ay = 66;
	
	  // Round the mapped number.
	  var bx = round(map(mouseX, 0, 100, 0,5));
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
