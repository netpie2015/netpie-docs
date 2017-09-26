.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

get()
=====

ส่งค่าอาร์เรย์ของค่า [R, G, B, A] สำหรับพิกเซลใด ๆ หรือคว้าส่วนใดส่วนหนึ่งของรูปภาพ หากไม่มีพารามิเตอร์ระบุไว้รูปภาพทั้งหมดจะถูกส่งคืน ใช้พารามิเตอร์ x และ y เพื่อรับค่าหนึ่งพิกเซล รับส่วนของหน้าต่างการแสดงผลโดยการระบุพารามิเตอร์ w และ h เพิ่มเติม เมื่อได้รับรูปภาพพารามิเตอร์ x และ y กำหนดพิกัดสำหรับมุมซ้ายบนของภาพโดยไม่คำนึงถึง imageMode () ในปัจจุบัน 
หากพิกเซลที่ขออยู่นอกกรอบภาพจะส่งกลับ [0,0,0,255] เพื่อให้ได้ตัวเลขที่ปรับขนาดตามช่วงสีปัจจุบันและคำนึงถึง colorMode ให้ใช้ getColor แทนการรับ 
การรับสีของพิกเซลเพียงจุดเดียวด้วย get (x, y) เป็นเรื่องง่าย แต่ไม่เร็วเท่าการคว้าข้อมูลโดยตรงจากพิกเซล [] (x, y) โดยใช้พิกเซล [] ที่มีความหนาแน่นของพิกเซล d คือ var off = (y * width + x) * d * 4; [pixels[off], pixels[off+1], pixels[off+2], pixels[off+3]] 
ดูข้อมูลอ้างอิงสำหรับพิกเซล [] สำหรับข้อมูลเพิ่มเติม

.. Returns an array of [R,G,B,A] values for any pixel or grabs a section of
.. an image. If no parameters are specified, the entire image is returned.
.. Use the x and y parameters to get the value of one pixel. Get a section of
.. the display window by specifying additional w and h parameters. When
.. getting an image, the x and y parameters define the coordinates for the
.. upper-left corner of the image, regardless of the current imageMode().
.. 
.. If the pixel requested is outside of the image window, [0,0,0,255] is
.. returned. To get the numbers scaled according to the current color ranges
.. and taking into account colorMode, use getColor instead of get.
.. 
.. Getting the color of a single pixel with get(x, y) is easy, but not as fast
.. as grabbing the data directly from pixels[]. The equivalent statement to
.. get(x, y) using pixels[] with pixel density d is
.. 
.. var off = (y * width + x) * d * 4;
.. [pixels[off],
.. pixels[off+1],
.. pixels[off+2],
.. pixels[off+3]]
.. 
.. See the reference for pixels[] for more information.

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

- Array.<Number>,p5.Image: ค่าพิกเซลที่ x, y ในรูปแบบอาร์เรย์ [R, G, B, A] หรือ p5.Image

.. Array.<Number>,p5.Image: values of pixel at x,y in array format [R, G, B, A] or p5.Image

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var img;
	function preload() {
	  img = loadImage("assets/rockies.jpg");
	}
	function setup() {
	  image(img, 0, 0);
	  var c = get();
	  image(c, width/2, 0);
	}

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	var img;
	function preload() {
	  img = loadImage("assets/rockies.jpg");
	}
	function setup() {
	  image(img, 0, 0);
	  var c = get(50, 90);
	  fill(c);
	  noStroke();
	  rect(25, 25, 50, 50);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
