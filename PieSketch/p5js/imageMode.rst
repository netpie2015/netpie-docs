.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

imageMode()
===========

โหลดรูปภาพจากเส้นทางและสร้าง p5.Image จากไฟล์

ภาพอาจไม่สามารถใช้งานได้ทันทีสำหรับการแสดงผลหากคุณต้องการให้แน่ใจว่ารูปภาพพร้อมใช้งานแล้วก่อนที่จะทำอะไรให้ทำโหลด loadImage () ใน preload () นอกจากนี้คุณยังสามารถจัดหาฟังก์ชันการโทรกลับเพื่อจัดการกับภาพเมื่อพร้อม

เส้นทางไปยังรูปภาพต้องสัมพันธ์กับไฟล์ HTML ที่ลิงก์ในร่างของคุณ การโหลดรูปภาพจาก URL หรือสถานที่ห่างไกลอื่น ๆ อาจถูกบล็อกเนื่องจากความปลอดภัยภายในของเบราเซอร์ของคุณ

.. Loads an image from a path and creates a p5.Image from it.
.. The image may not be immediately available for rendering If you want to ensure that the image is ready before doing anything with it, place the loadImage() call in preload(). You may also supply a callback function to handle the image when it's ready.
.. The path to the image should be relative to the HTML file that links in your sketch. Loading an image from a URL or other remote location may be blocked due to your browser's built-in security.

**รูปแบบการใช้งาน**

loadImage(path,[successCallback],[failureCallback])

**พารามิเตอร์**

- ``path``  สตริง: เส้นทางของรูปภาพที่จะโหลด

- ``successCallback``  ฟังก์ชั่น (p5.Image): ฟังก์ชั่นที่จะเรียกเมื่อภาพถูกโหลด จะถูกส่งผ่าน p5.Image

- ``failureCallback``  ฟังก์ชัน (เหตุการณ์): เรียกว่ามีข้อผิดพลาดของเหตุการณ์ถ้าไม่สามารถโหลดภาพ

.. ``path``  String: Path of the image to be loaded
.. ``successCallback``  function(p5.Image): Function to be called once the image is loaded. Will be passed the p5.Image.
.. ``failureCallback``  Function(Event): called with event error if the image fails to load.

**ค่าที่ส่งออกมา**

- p5.Image: วัตถุ p5.Image

.. p5.Image: the p5.Image object

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
