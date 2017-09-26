.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

get()
=====

รับพื้นที่พิกเซลจากภาพ ถ้าไม่ผ่าน params ภาพทั้งหมดที่ถูกส่งกลับถ้า x และ y เป็น params เดียวที่ส่งผ่าน pixel เดียวจะถูกแยกออกถ้า params ทั้งหมดถูกส่งผ่านพื้นที่สี่เหลี่ยมผืนผ้าจะถูกแยกและ p5 จะถูกส่งกลับ ส่งกลับไม่ได้กำหนดหากพื้นที่อยู่นอกขอบเขตของรูปภาพ

.. Get a region of pixels from an image.
.. If no params are passed, those whole image is returned,
.. if x and y are the only params passed a single pixel is extracted
.. if all params are passed a rectangle region is extracted and a p5.Image
.. is returned.
.. Returns undefined if the region is outside the bounds of the image
**รูปแบบการใช้งาน**

get ( [x], [y], [w], [h] )

**พารามิเตอร์**

- ``x``  Number: พิกัด x ของพิกเซล

- ``y``  Number: y พิกัดของพิกเซล

- ``w``  Number: ความกว้าง

- ``h``  Number: ความสูง

.. ``x``  Number: x-coordinate of the pixel
.. ``y``  Number: y-coordinate of the pixel
.. ``w``  Number: width
.. ``h``  Number: height

**ค่าที่ส่งออกมา**

- Array.<Number>,Color,p5.Image: สีของพิกเซลที่ x, y ในรูปแบบอาร์เรย์ [R, G, B, A] หรือ p5.Image

.. Array.<Number>,Color,p5.Image: color of pixel at x,y in array format [R, G, B, A] or p5.Image

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var myImage;
	var c;
	
	function preload() {
	  myImage = loadImage("assets/rockies.jpg");
	}
	
	function setup() {
	  background(myImage);
	  noStroke();
	  c = myImage.get(60, 90);
	  fill(c);
	  rect(25, 25, 50, 50);
	}
	
	//get() returns color here

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
