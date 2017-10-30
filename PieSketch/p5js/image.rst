.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

image()
=======

วาดภาพลงในผืนผ้าใบ p5.js

ฟังก์ชั่นนี้สามารถใช้ได้กับพารามิเตอร์ต่างกัน การใช้งานที่ง่ายที่สุดต้องใช้พารามิเตอร์เพียงสามอย่าง ได้แก่ img, x และ y-where (x, y) คือตำแหน่งของภาพ คุณสามารถเพิ่มพารามิเตอร์สองตัวเพื่อระบุความกว้างและความสูงของภาพได้

ฟังก์ชั่นนี้สามารถใช้ได้กับพารามิเตอร์จำนวนแปดตัว เพื่อแยกความแตกต่างระหว่างพารามิเตอร์เหล่านี้ p5.js ใช้ภาษาของ "สี่เหลี่ยมผืนผ้าปลายทาง" (ซึ่งตรงกับ "dx", "dy" ฯลฯ ) และ "ภาพต้นฉบับ" (ซึ่งตรงกับ "sx", "sy" ฯลฯ ) ด้านล่าง การระบุมิติข้อมูล "ภาพต้นฉบับ" จะเป็นประโยชน์เมื่อคุณต้องการแสดงส่วนย่อยของภาพต้นฉบับแทนสิ่งที่ทั้งตัว นี่เป็นแผนภาพที่จะอธิบายเพิ่มเติม:

.. raw:: html

    <center><image src="https://p5js.org/reference/assets/drawImage.png"></center>

.. Draw an image to the p5.js canvas.
.. This function can be used with different numbers of parameters. The simplest use requires only three parameters: img, x, and y—where (x, y) is the position of the image. Two more parameters can optionally be added to specify the width and height of the image.
.. This function can also be used with all eight Number parameters. To differentiate between all these parameters, p5.js uses the language of "destination rectangle" (which corresponds to "dx", "dy", etc.) and "source image" (which corresponds to "sx", "sy", etc.) below. Specifying the "source image" dimensions can be useful when you want to display a subsection of the source image instead of the whole thing. Here's a diagram to explain further: 

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
