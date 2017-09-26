.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

noiseSeed()
===========

กำหนดค่าเมล็ดสำหรับ noise () โดยค่าเริ่มต้น noise () จะให้ผลลัพธ์ที่แตกต่างกันในแต่ละครั้งที่มีการเรียกใช้โปรแกรม ตั้ง ค่า พารามิเตอร์ให้เป็นค่าคงที่เพื่อส่งคืนหมายเลขแบบสุ่มหลอกเดียวกันทุกครั้งที่มีการเรียกใช้ซอฟต์แวร์

.. Sets the seed value for noise(). By default, noise()
.. produces different results each time the program is run. Set the
.. value parameter to a constant to return the same pseudo-random
.. numbers each time the software is run.
**รูปแบบการใช้งาน**

noiseSeed ( seed )

**พารามิเตอร์**

- ``seed``  Number: ค่าเมล็ด

.. ``seed``  Number: the seed value

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var xoff = 0.0;
	
	function setup() {
	  noiseSeed(99);
	  stroke(0, 10);
	}
	
	function draw() {
	  xoff = xoff + .01;
	  var n = noise(xoff) * width;
	  line(n, 0, n, height);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
