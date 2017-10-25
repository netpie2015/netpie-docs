.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

noSmooth()
==========

วาดรูปทรงเรขาคณิตทั้งหมดที่มีขอบขรุขระ (aliased) โปรดทราบว่า smooth () มีการใช้งานโดยค่าเริ่มต้นดังนั้นจึงจำเป็นต้องเรียก noSmooth () เพื่อปิดการปรับให้เรียบรูปเรขาคณิตรูปภาพและแบบอักษร

.. Draws all geometry with jagged (aliased) edges. Note that smooth() is active by default, so it is necessary to call noSmooth() to disable smoothing of geometry, images, and fonts.

**รูปแบบการใช้งาน**

noSmooth()

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	background(0);
    noStroke();
    smooth();
    ellipse(30, 48, 36, 36);
    noSmooth();
    ellipse(70, 48, 36, 36);
	</script>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
