.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

imageMode()
===========

โหลดรูปภาพจากเส้นทางและสร้าง p5.Image จากไฟล์

ภาพอาจไม่สามารถใช้งานได้ทันทีสำหรับการแสดงผลหากคุณต้องการให้แน่ใจว่ารูปภาพพร้อมใช้งานแล้วก่อนที่จะทำอะไรให้ทำโหลด loadImage () ใน preload () นอกจากนี้คุณยังสามารถจัดหาฟังก์ชันการโทรกลับเพื่อจัดการกับภาพเมื่อพร้อม

เส้นทางไปยังรูปภาพต้องสัมพันธ์กับไฟล์ HTML ที่ลิงก์ในร่างของคุณ การโหลดรูปภาพจาก URL หรือสถานที่ห่างไกลอื่น ๆ อาจถูกบล็อกเนื่องจากความปลอดภัยภายในของเบราเซอร์ของคุณ

.. Set image mode. Modifies the location from which images are drawn by changing the way in which parameters given to image() are interpreted. The default mode is imageMode(CORNER), which interprets the second and third parameters of image() as the upper-left corner of the image. If two additional parameters are specified, they are used to set the image's width and height.
.. imageMode(CORNERS) interprets the second and third parameters of image() as the location of one corner, and the fourth and fifth parameters as the opposite corner.
.. imageMode(CENTER) interprets the second and third parameters of image() as the image's center point. If two additional parameters are specified, they are used to set the image's width and height.

**รูปแบบการใช้งาน**

imageMode(mode)

**พารามิเตอร์**

- ``mode``  ค่าคงที่: ทั้ง CORNER, CORNERS หรือ CENTER

.. ``mode``  Constant: either CORNER, CORNERS, or CENTER

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var img;
    function preload() {
        img = loadImage("assets/bricks.jpg");
    }
    function setup() {
        imageMode(CORNER);
        image(img, 10, 10, 50, 50);
    }
	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var img;
    function preload() {
        img = loadImage("assets/bricks.jpg");
    }
    function setup() {
        imageMode(CORNERS);
        image(img, 10, 10, 90, 40);
    }
	</script>

	<br><br>

    <script type="text/p5" data-autoplay data-hide-sourcecode>
	var img;
    function preload() {
        img = loadImage("assets/bricks.jpg");
    }
    function setup() {
        imageMode(CENTER);
        image(img, 50, 50, 80, 80);
    }
	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
