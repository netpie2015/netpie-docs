.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

createImage()
=============

สร้าง p5.Image ใหม่ (ประเภทข้อมูลสำหรับจัดเก็บภาพ) นี่เป็นบัฟเฟอร์ใหม่ของพิกเซลที่เล่นด้วย ตั้งค่าขนาดของบัฟเฟอร์ที่มีพารามิเตอร์ความกว้างและความสูง 
พิกเซลให้การเข้าถึงอาร์เรย์ที่มีค่าพิกเซลทั้งหมดในหน้าต่างแสดงผล ค่าเหล่านี้คือตัวเลข อาร์เรย์นี้เป็นขนาด (รวมถึงปัจจัยที่เหมาะสมสำหรับ pixelDensity) ของหน้าต่างแสดง x4 แทนค่า R, G, B, A เพื่อให้แต่ละพิกเซลเคลื่อนที่จากซ้ายไปขวาในแต่ละแถวจากนั้นให้ลดแต่ละคอลัมน์ ดูพิกเซลสำหรับข้อมูลเพิ่มเติม นอกจากนี้ยังอาจจะง่ายกว่าที่จะใช้ set () หรือ get () 
ก่อนที่จะเข้าถึงพิกเซลของรูปภาพข้อมูลต้องโหลดด้วยฟังก์ชัน loadPixels () หลังจากที่ข้อมูลอาร์เรย์ได้รับการแก้ไขต้องใช้ฟังก์ชัน updatePixels () เพื่ออัพเดตการเปลี่ยนแปลง

.. Creates a new p5.Image (the datatype for storing images). This provides a
.. fresh buffer of pixels to play with. Set the size of the buffer with the
.. width and height parameters.
.. 
.. .pixels gives access to an array containing the values for all the pixels
.. in the display window.
.. These values are numbers. This array is the size (including an appropriate
.. factor for the pixelDensity) of the display window x4,
.. representing the R, G, B, A values in order for each pixel, moving from
.. left to right across each row, then down each column. See .pixels for
.. more info. It may also be simpler to use set() or get().
.. 
.. Before accessing the pixels of an image, the data must loaded with the
.. loadPixels() function. After the array data has been modified, the
.. updatePixels() function must be run to update the changes.

**รูปแบบการใช้งาน**

createImage ( width, height )

**พารามิเตอร์**

- ``width``  Integer: ความกว้างเป็นพิกเซล

- ``height``  Integer: ความสูงเป็นพิกเซล

.. ``width``  Integer: width in pixels
.. ``height``  Integer: height in pixels

**ค่าที่ส่งออกมา**

- p5.Image: วัตถุ p5.Image

.. p5.Image: the p5.Image object

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	img = createImage(66, 66);
	img.loadPixels();
	for (i = 0; i < img.width; i++) {
	  for (j = 0; j < img.height; j++) {
	    img.set(i, j, color(0, 90, 102));
	  }
	}
	img.updatePixels();
	image(img, 17, 17);

	</script>

	<br><br>

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

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	var pink = color(255, 102, 204);
	img = createImage(66, 66);
	img.loadPixels();
	var d = pixelDensity();
	var halfImage = 4 * (width * d) * (height/2 * d);
	for (var i = 0; i < halfImage; i+=4) {
	  img.pixels[i] = red(pink);
	  img.pixels[i+1] = green(pink);
	  img.pixels[i+2] = blue(pink);
	  img.pixels[i+3] = alpha(pink);
	}
	img.updatePixels();
	image(img, 17, 17);

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
