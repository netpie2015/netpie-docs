.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

map()
=====

ทำแผนที่ใหม่จากช่วงหนึ่งไปยังอีกที่หนึ่ง 
ในตัวอย่างแรกด้านบนหมายเลข 25 จะถูกแปลงจากค่าในช่วง 0 ถึง 100 เป็นค่าที่อยู่ในช่วงตั้งแต่ขอบด้านซ้ายของหน้าต่าง (0) ไปยังขอบด้านขวา (กว้าง)

.. Re-maps a number from one range to another.
.. 
.. In the first example above, the number 25 is converted from a value in the
.. range of 0 to 100 into a value that ranges from the left edge of the
.. window (0) to the right edge (width).

**รูปแบบการใช้งาน**

map ( value, start1, stop1, start2, stop2 )

**พารามิเตอร์**

- ``value``  Number: ค่าที่เข้ามาที่จะแปลง

- ``start1``  Number: ขอบเขตล่างของช่วงปัจจุบันของค่า

- ``stop1``  Number: ขอบเขตบนของช่วงปัจจุบันของค่า

- ``start2``  Number: ขอบเขตล่างของช่วงเป้าหมายของค่า

- ``stop2``  Number: ขอบเขตบนของช่วงเป้าหมายของค่า

.. ``value``  Number: the incoming value to be converted
.. ``start1``  Number: lower bound of the value's current range
.. ``stop1``  Number: upper bound of the value's current range
.. ``start2``  Number: lower bound of the value's target range
.. ``stop2``  Number: upper bound of the value's target range

**ค่าที่ส่งออกมา**

- Number: หมายเลขที่สำรองใหม่

.. Number: remapped number

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	    var value = 25;
	    var m = map(value, 0, 100, 0, width);
	    ellipse(m, 50, 10, 10);
	        function setup() {
	      noStroke();
	    }
	
	    function draw() {
	      background(204);
	      var x1 = map(mouseX, 0, width, 25, 75);
	      ellipse(x1, 25, 25, 25);
	      var x2 = map(mouseX, 0, width, 0, 100);
	      ellipse(x2, 75, 25, 25);
	    }
	  

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
