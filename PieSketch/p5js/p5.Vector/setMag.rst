.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

setMag()
========

กำหนดขนาดของเวกเตอร์นี้เป็นค่าที่ใช้สำหรับพารามิเตอร์ len

.. Set the magnitude of this vector to the value used for the len
.. parameter.

**รูปแบบการใช้งาน**

setMag ( len )

**พารามิเตอร์**

- ``len``  number: ความยาวใหม่สำหรับเวกเตอร์นี้

.. ``len``  number: the new length for this vector

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var v = createVector(10, 20, 2);
	// v has components [10.0, 20.0, 2.0]
	v.setMag(10);
	// v's components are set to [6.0, 8.0, 0.0]

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
