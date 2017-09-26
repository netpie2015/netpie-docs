.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

filter()
========

ใช้ตัวกรองภาพกับ p5.Image

.. Applies an image filter to a p5.Image
**รูปแบบการใช้งาน**

filter ( operation, value )

**พารามิเตอร์**

- ``operation``  String: หนึ่งในเกณฑ์, สีเทา, กลับ, posterize, ทึบแสงกัดเซาะขยายและเบลอ ดู Filters.js สำหรับเอกสารในตัวกรองที่มีอยู่แต่ละตัว

- ``value``  Number,undefined: 

.. ``operation``  String: one of threshold, gray, invert, posterize, opaque
                          erode, dilate and blur. See Filters.js for docs on
                          each available filter
.. ``value``  Number,undefined: 

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var photo1;
	var photo2;
	
	function preload() {
	  photo1 = loadImage("assets/rockies.jpg");
	  photo2 = loadImage("assets/rockies.jpg");
	}
	
	function setup() {
	  photo2.filter("gray");
	  image(photo1, 0, 0);
	  image(photo2, width/2, 0);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
