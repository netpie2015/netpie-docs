.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

resizeCanvas()
==============

ปรับขนาดผ้าใบเพื่อให้ได้ความกว้างและความสูง ผืนผ้าใบจะถูกล้างและวาดจะเรียกทันทีเพื่อให้ร่างภาพสามารถแสดงผลใหม่ในผืนผ้าใบที่ปรับขนาดได้

.. Resizes the canvas to given width and height. The canvas will be cleared
.. and draw will be called immediately, allowing the sketch to re-render itself
.. in the resized canvas.

**รูปแบบการใช้งาน**

resizeCanvas ( w, h, noRedraw )

**พารามิเตอร์**

- ``w``  Number: ความกว้างของผ้าใบ

- ``h``  Number: ความสูงของผ้าใบ

- ``noRedraw``  Boolean: อย่าวาดภาพผืนผ้าใบทันที

.. ``w``  Number: width of the canvas
.. ``h``  Number: height of the canvas
.. ``noRedraw``  Boolean: don't redraw the canvas immediately

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  createCanvas(windowWidth, windowHeight);
	}
	
	function draw() {
	 background(0, 100, 200);
	}
	
	function windowResized() {
	  resizeCanvas(windowWidth, windowHeight);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
