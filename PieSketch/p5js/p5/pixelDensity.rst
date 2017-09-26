.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

pixelDensity()
==============

ตั้งค่าการปรับพิกเซลสำหรับการแสดงความหนาแน่นของพิกเซลสูง โดยค่าเริ่มต้นความหนาแน่นของพิกเซลถูกตั้งค่าให้ตรงกับความหนาแน่นของการแสดงผลให้เรียก pixelDensity (1) เพื่อปิดการทำงานนี้ การเรียก pixelDensity () ที่ไม่มีอาร์กิวเมนต์จะส่งกลับความหนาแน่นของพิกเซลในปัจจุบันของร่าง

.. Sets the pixel scaling for high pixel density displays. By default
.. pixel density is set to match display density, call pixelDensity(1)
.. to turn this off. Calling pixelDensity() with no arguments returns
.. the current pixel density of the sketch.
**รูปแบบการใช้งาน**

pixelDensity ( [val] )

**พารามิเตอร์**

- ``val``  Number: ไม่ว่าจะเป็นภาพร่างหรือขนาดเท่าไร

.. ``val``  Number: whether or how much the sketch should scale

**ค่าที่ส่งออกมา**

- Number: ความหนาแน่นของพิกเซลในปัจจุบันของร่าง

.. Number: current pixel density of the sketch

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  pixelDensity(1);
	  createCanvas(100, 100);
	  background(200);
	  ellipse(width/2, height/2, 50, 50);
	}

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  pixelDensity(3.0);
	  createCanvas(100, 100);
	  background(200);
	  ellipse(width/2, height/2, 50, 50);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
