.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

mag()
=====

คำนวณขนาด (หรือความยาว) ของเวกเตอร์ เวกเตอร์เป็นทิศทางในพื้นที่ที่ใช้กันโดยทั่วไปในด้านกราฟิกคอมพิวเตอร์และพีชคณิตเชิงเส้น เนื่องจากไม่มีตำแหน่ง "เริ่มต้น" ขนาดของเวกเตอร์อาจถือได้ว่าเป็นระยะทางจากพิกัด 0,0 ถึงค่า x, y ของมัน ดังนั้น mag () เป็นทางลัดสำหรับการเขียน dist (0, 0, x, y)

.. Calculates the magnitude (or length) of a vector. A vector is a direction
.. in space commonly used in computer graphics and linear algebra. Because it
.. has no "start" position, the magnitude of a vector can be thought of as
.. the distance from the coordinate 0,0 to its x,y value. Therefore, mag() is
.. a shortcut for writing dist(0, 0, x, y).

**รูปแบบการใช้งาน**

mag ( a, b )

**พารามิเตอร์**

- ``a``  Number: ค่าแรก

- ``b``  Number: ค่าที่สอง

.. ``a``  Number: first value
.. ``b``  Number: second value

**ค่าที่ส่งออกมา**

- Number: ขนาดของเวกเตอร์จาก (0,0) ถึง (a, b)

.. Number: magnitude of vector from (0,0) to (a,b)

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var x1 = 20;
	  var x2 = 80;
	  var y1 = 30;
	  var y2 = 70;
	
	  line(0, 0, x1, y1);
	  print(mag(x1, y1));  // Prints "36.05551275463989"
	  line(0, 0, x2, y1);
	  print(mag(x2, y1));  // Prints "85.44003745317531"
	  line(0, 0, x1, y2);
	  print(mag(x1, y2));  // Prints "72.80109889280519"
	  line(0, 0, x2, y2);
	  print(mag(x2, y2));  // Prints "106.3014581273465"
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
