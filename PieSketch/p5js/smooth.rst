.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

smooth()
========

วาดรูปทรงเรขาคณิตทั้งหมดที่มีขอบเรียบ (anti-aliased) smooth () จะช่วยปรับปรุงคุณภาพของภาพที่ปรับขนาดได้ โปรดทราบว่า smooth () มีการใช้งานโดยค่าเริ่มต้น noSmooth () สามารถใช้เพื่อปิดการปรับรูปทรงเรขาคณิตภาพและแบบอักษรได้

.. Draws all geometry with smooth (anti-aliased) edges. smooth() will also improve image quality of resized images. Note that smooth() is active by default; noSmooth() can be used to disable smoothing of geometry, images, and fonts.

**รูปแบบการใช้งาน**

smooth()

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	background(0);
    noStroke();
    smooth();
    ellipse(30, 48, 36, 36);
    noSmooth();
    ellipse(70, 48, 36, 36);
	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
