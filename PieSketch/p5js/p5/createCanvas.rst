.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

createCanvas()
==============

สร้างองค์ประกอบผ้าใบในเอกสารและกำหนดขนาดของภาพในพิกเซล วิธีนี้ควรจะเรียกว่าเพียงครั้งเดียวเมื่อเริ่มต้นของการติดตั้ง การเรียก createCanvas มากกว่าหนึ่งครั้งในร่างจะส่งผลให้เกิดพฤติกรรมที่ไม่อาจคาดเดาได้มาก ถ้าคุณต้องการภาพวาดมากกว่าหนึ่งภาพคุณสามารถใช้ createGraphics (ซ่อนไว้โดยค่าเริ่มต้น แต่สามารถแสดงได้) 
ความกว้างของตัวแปรระบบและความสูงถูกกำหนดโดยพารามิเตอร์ที่ส่งผ่านไปยังฟังก์ชันนี้ หากไม่ได้ใช้ createCanvas () หน้าต่างจะได้รับขนาดเริ่มต้น 100x100 พิกเซล 
สำหรับวิธีการเพิ่มเติมในการวางผืนผ้าใบให้ดูที่การ วางตำแหน่ง หน้าวิกิพีเดีย ผ้าใบ

.. Creates a canvas element in the document, and sets the dimensions of it
.. in pixels. This method should be called only once at the start of setup.
.. Calling createCanvas more than once in a sketch will result in very
.. unpredicable behavior. If you want more than one drawing canvas
.. you could use createGraphics (hidden by default but it can be shown).
.. 
.. The system variables width and height are set by the parameters passed
.. to this function. If createCanvas() is not used, the window will be
.. given a default size of 100x100 pixels.
.. 
.. For more ways to position the canvas, see the
.. 
.. positioning the canvas wiki page.
**รูปแบบการใช้งาน**

createCanvas ( w, h, [renderer] )

**พารามิเตอร์**

- ``w``  Number: ความกว้างของผ้าใบ

- ``h``  Number: ความสูงของผ้าใบ

- ``renderer``  Constant: ทั้ง P2D หรือ WEBGL

.. ``w``  Number: width of the canvas
.. ``h``  Number: height of the canvas
.. ``renderer``  Constant: either P2D or WEBGL

**ค่าที่ส่งออกมา**

- HTMLCanvasElement: ผ้าใบที่สร้างขึ้น

.. HTMLCanvasElement: canvas generated

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  createCanvas(100, 50);
	  background(153);
	  line(0, 0, width, height);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
