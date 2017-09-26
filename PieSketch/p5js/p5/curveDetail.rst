.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

curveDetail()
=============

ตั้งค่าความละเอียดที่เส้นโค้งแสดง ค่าดีฟอลต์คือ 20

.. Sets the resolution at which curves display.
.. The default value is 20.
**รูปแบบการใช้งาน**

curveDetail ( resolution )

**พารามิเตอร์**

- ``resolution``  Number: ของเส้นโค้ง

.. ``resolution``  Number: of the curves

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	background(204);
	curveDetail(20);
	curve(5, 26, 5, 26, 73, 24, 73, 61);

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
