.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

bezierDetail()
==============

ตั้งค่าความละเอียดที่ Beziers แสดง ค่าดีฟอลต์คือ 20

.. Sets the resolution at which Beziers display.
.. The default value is 20.
**รูปแบบการใช้งาน**

bezierDetail ( detail )

**พารามิเตอร์**

- ``detail``  Number: ความละเอียดของเส้นโค้ง

.. ``detail``  Number: resolution of the curves

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	background(204);
	bezierDetail(50);
	bezier(85, 20, 10, 10, 90, 90, 15, 80);

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
