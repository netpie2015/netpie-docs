.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

set()
=====

ตั้งค่าสีของพิกเซลเดียวหรือเขียนภาพลงใน p5.Image นี้ โปรดทราบว่าสำหรับพิกเซลจำนวนมากจะช้ากว่าการจัดการอาร์เรย์ของพิกเซลโดยตรงและจากนั้นเรียกใช้ updatePixels ()

.. Set the color of a single pixel or write an image into
.. this p5.Image.
.. Note that for a large number of pixels this will
.. be slower than directly manipulating the pixels array
.. and then calling updatePixels().
**รูปแบบการใช้งาน**

set ( x, y, a )

**พารามิเตอร์**

- ``x``  Number: พิกัด x ของพิกเซล

- ``y``  Number: y พิกัดของพิกเซล

- ``a``  Number,Array,Object: ค่า grayscale | อาร์เรย์พิกเซล p5.Color | ภาพที่จะคัดลอก

.. ``x``  Number: x-coordinate of the pixel
.. ``y``  Number: y-coordinate of the pixel
.. ``a``  Number,Array,Object: grayscale value | pixel array |
                               a p5.Color | image to copy

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	img = createImage(66, 66);
	img.loadPixels();
	for (i = 0; i < img.width; i++) {
	  for (j = 0; j < img.height; j++) {
	    img.set(i, j, color(0, 90, 102, i % img.width * 2));
	  }
	}
	img.updatePixels();
	image(img, 17, 17);
	image(img, 34, 34);

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
