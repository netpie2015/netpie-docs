.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

image()
=======

โหลดรูปภาพจากเส้นทางและสร้าง p5.Image จากไฟล์

ภาพอาจไม่สามารถใช้งานได้ทันทีสำหรับการแสดงผลหากคุณต้องการให้แน่ใจว่ารูปภาพพร้อมใช้งานแล้วก่อนที่จะทำอะไรให้ทำโหลด loadImage () ใน preload () นอกจากนี้คุณยังสามารถจัดหาฟังก์ชันการโทรกลับเพื่อจัดการกับภาพเมื่อพร้อม

เส้นทางไปยังรูปภาพต้องสัมพันธ์กับไฟล์ HTML ที่ลิงก์ในร่างของคุณ การโหลดรูปภาพจาก URL หรือสถานที่ห่างไกลอื่น ๆ อาจถูกบล็อกเนื่องจากความปลอดภัยภายในของเบราเซอร์ของคุณ

.. Loads an image from a path and creates a p5.Image from it.
.. The image may not be immediately available for rendering If you want to ensure that the image is ready before doing anything with it, place the loadImage() call in preload(). You may also supply a callback function to handle the image when it's ready.
.. The path to the image should be relative to the HTML file that links in your sketch. Loading an image from a URL or other remote location may be blocked due to your browser's built-in security.

**รูปแบบการใช้งาน**

image(img,x,y,[width],[height])

image(img,dx,dy,dWidth,dHeight,sx,sy,[sWidth],[sHeight])

**พารามิเตอร์**

- ``img``  p5.Image | p5.Graphics: ภาพที่จะแสดง

- ``x``  ตัวเลข: พิกัด x ที่มุมซ้ายบนของภาพ

- ``y``  ตัวเลข: พิกัด y ที่มุมซ้ายบนของภาพ

- ``width``  ตัวเลข: ความกว้างในการวาดภาพ

- ``height``  ตัวเลข: ความสูงในการวาดภาพ

- ``dx``  ตัวเลข: พิกัด x ของสี่เหลี่ยมผืนผ้าปลายทางที่จะวาดภาพต้นฉบับ

- ``dy``  ตัวเลข: พิกัด y ของสี่เหลี่ยมผืนผ้าปลายทางที่จะวาดภาพต้นฉบับ

- ``dWidth``  ตัวเลข: ความกว้างของสี่เหลี่ยมผืนผ้าปลายทาง

- ``dHeight``  ตัวเลข: ความสูงของสี่เหลี่ยมผืนผ้าปลายทาง

- ``sx``  ตัวเลข: พิกัด x ของส่วนย่อยของภาพต้นฉบับเพื่อวาดลงในสี่เหลี่ยมผืนผ้าปลายทาง

- ``sy``  ตัวเลข: พิกัด y ของส่วนย่อยของภาพต้นฉบับเพื่อวาดลงในสี่เหลี่ยมผืนผ้าปลายทาง

- ``sWidth``  ตัวเลข: ความกว้างของส่วนย่อยของภาพต้นฉบับเพื่อวาดลงในสี่เหลี่ยมผืนผ้าปลายทาง

- ``sHeight``  ตัวเลข: ความสูงของส่วนย่อยของภาพต้นฉบับเพื่อวาดลงในสี่เหลี่ยมผืนผ้าปลายทาง

.. ``img``  p5.Image|p5.Graphics: the image to display
.. ``x``  Number: the x-coordinate of the top-left corner of the image
.. ``y``  Number: the y-coordinate of the top-left corner of the image
.. ``width``  Number: the width to draw the image
.. ``height``  Number: the height to draw the image
.. ``dx``  Number: the x-coordinate of the destination rectangle in which to draw the source image
.. ``dy``  Number: the y-coordinate of the destination rectangle in which to draw the source image
.. ``dWidth``  Number: the width of the destination rectangle
.. ``dHeight``  Number: the height of the destination rectangle
.. ``sx``  Number: the x-coordinate of the subsection of the source image to draw into the destination rectangle
.. ``sy``  Number: the y-coordinate of the subsection of the source image to draw into the destination rectangle
.. ``sWidth``  Number: the width of the subsection of the source image to draw into the destination rectangle
.. ``sHeight``  Number: the height of the subsection of the source image to draw into the destination rectangle


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var img;
    function preload() {
        img = loadImage("assets/laDefense.jpg");
    }
    function setup() {
        // Top-left corner of the img is at (0, 0)
        // Width and height are the img's original width and height
        image(img, 0, 0);
    }
	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var img;
    function preload() {
        img = loadImage("assets/laDefense.jpg");
    }
    function setup() {
        background(50);
        // Top-left corner of the img is at (10, 10)
        // Width and height are 50 x 50
        image(img, 10, 10, 50, 50);
    }
	</script>

	<br><br>

    <script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
        // Here, we use a callback to display the image after loading
        loadImage("assets/laDefense.jpg", function(img) {
            image(img, 0, 0);
        });
    }
	</script>

	<br><br>

    <script type="text/p5" data-autoplay data-hide-sourcecode>
	var img;
    function preload() {
        img = loadImage("assets/gradient.png");
    }
    function setup() {
        // 1. Background image
        // Top-left corner of the img is at (0, 0)
        // Width and height are the img's original width and height, 100 x 100
        image(img, 0, 0);
        // 2. Top right image
        // Top-left corner of destination rectangle is at (50, 0)
        // Destination rectangle width and height are 40 x 20
        // The next parameters are relative to the source image:
        // - Starting at position (50, 50) on the source image, capture a 50 x 50
        // subsection
        // - Draw this subsection to fill the dimensions of the destination rectangle
        image(img, 50, 0, 40, 20, 50, 50, 50, 50);
    }
	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
