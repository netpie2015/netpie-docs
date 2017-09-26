.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

createGraphics()
================

สร้างและส่งกลับอ็อบเจ็กต์ p5.Renderer ใหม่ ใช้คลาสนี้ถ้าคุณต้องการวาดลงในบัฟเฟอร์กราฟิกนอกจอ พารามิเตอร์ทั้งสองกำหนดความกว้างและความสูงเป็นพิกเซล

.. Creates and returns a new p5.Renderer object. Use this class if you need
.. to draw into an off-screen graphics buffer. The two parameters define the
.. width and height in pixels.

**รูปแบบการใช้งาน**

createGraphics ( w, h, [renderer] )

**พารามิเตอร์**

- ``w``  Number: ความกว้างของบัฟเฟอร์กราฟิก offscreen

- ``h``  Number: ความสูงของบัฟเฟอร์กราฟิก offscreen

- ``renderer``  Constant: ทั้งค่าเริ่มต้นของ P2D หรือ WEBGL ที่ไม่ได้กำหนดไว้สำหรับ p2d

.. ``w``  Number: width of the offscreen graphics buffer
.. ``h``  Number: height of the offscreen graphics buffer
.. ``renderer``  Constant: either P2D or WEBGL undefined defaults to p2d

**ค่าที่ส่งออกมา**

- p5.Graphics: บัฟเฟอร์กราฟิก offscreen

.. p5.Graphics: offscreen graphics buffer

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var pg;
	function setup() {
	  createCanvas(100, 100);
	  pg = createGraphics(100, 100);
	}
	function draw() {
	  background(200);
	  pg.background(100);
	  pg.noStroke();
	  pg.ellipse(pg.width/2, pg.height/2, 50, 50);
	  image(pg, 50, 50);
	  image(pg, 0, 0, 50, 50);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
