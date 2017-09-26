.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

mask()
======

มาสก์ส่วนหนึ่งของรูปภาพจากการแสดงโดยการโหลดรูปภาพอื่นและใช้ช่องอัลฟาเป็นช่องอัลฟ่าสำหรับภาพนี้

.. Masks part of an image from displaying by loading another
.. image and using it's alpha channel as an alpha channel for
.. this image.
**รูปแบบการใช้งาน**

mask ( srcImage )

**พารามิเตอร์**

- ``srcImage``  p5.Image: ภาพต้นฉบับ

.. ``srcImage``  p5.Image: source image

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var photo, maskImage;
	function preload() {
	  photo = loadImage("assets/rockies.jpg");
	  maskImage = loadImage("assets/mask2.png");
	}
	
	function setup() {
	  createCanvas(100, 100);
	  photo.mask(maskImage);
	  image(photo, 0, 0);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
