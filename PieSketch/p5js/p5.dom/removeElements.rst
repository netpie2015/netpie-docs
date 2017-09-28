.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

removeElements()
================

ลบองค์ประกอบทั้งหมดที่สร้างโดย p5 ยกเว้นองค์ประกอบ canvas / graphics ที่สร้างโดย createCanvas หรือ createGraphics ตัวจัดการเหตุการณ์จะถูกลบออกและจะลบองค์ประกอบออกจาก DOM

.. Removes all elements created by p5, except any canvas / graphics
.. elements created by createCanvas or createGraphics.
.. Event handlers are removed, and element is removed from the DOM.

**รูปแบบการใช้งาน**

removeElements ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  createCanvas(100, 100);
	  createDiv('this is some text');
	  createP('this is a paragraph');
	}
	function mousePressed() {
	  removeElements(); // this will remove the div and p, not canvas
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
