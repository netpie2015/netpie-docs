.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

blend()
=======

คัดลอกพื้นที่พิกเซลจากภาพหนึ่งไปยังอีกภาพหนึ่งโดยใช้โหมดผสมผสานที่ระบุเพื่อดำเนินการ

.. Copies a region of pixels from one image to another, using a specified
.. blend mode to do the operation.
**รูปแบบการใช้งาน**

blend ( srcImage, sx, sy, sw, sh, dx, dy, dw, dh, blendMode )

**พารามิเตอร์**

- ``srcImage``  p5.Image,undefined: ภาพต้นฉบับ

- ``sx``  Integer: พิกัด X ของมุมซายบนของแหลง

- ``sy``  Integer: พิกัด Y ของมุมซายบนของแหลง

- ``sw``  Integer: ความกว้างของภาพต้นฉบับ

- ``sh``  Integer: ความสูงของภาพต้นฉบับ

- ``dx``  Integer: พิกัด X ของมุมบนซ้ายของปลายทาง

- ``dy``  Integer: พิกัด Y ของมุมบนซ้ายของปลายทาง

- ``dw``  Integer: ความกว้างของภาพปลายทาง

- ``dh``  Integer: ความสูงของภาพปลายทาง

- ``blendMode``  Integer: โหมดผสมผสานมีให้เลือกดังนี้: ปกติ | คูณ หน้าจอ การวางซ้อน | มืด เบาลง สีหลบ | การเผาไหม้ด้วยสี | ยาก - เบา แสงอ่อน | ความแตกต่าง การยกเว้น | สี | ความอิ่มตัว สี ความสว่าง http://blogs.adobe.com/webplatform/2013/01/28/blending-features-in-canvas/

.. ``srcImage``  p5.Image,undefined: source image
.. ``sx``  Integer: X coordinate of the source's upper left corner
.. ``sy``  Integer: Y coordinate of the source's upper left corner
.. ``sw``  Integer: source image width
.. ``sh``  Integer: source image height
.. ``dx``  Integer: X coordinate of the destination's upper left corner
.. ``dy``  Integer: Y coordinate of the destination's upper left corner
.. ``dw``  Integer: destination image width
.. ``dh``  Integer: destination image height
.. ``blendMode``  Integer: the blend mode

Available blend modes are: normal | multiply | screen | overlay |
           darken | lighten | color-dodge | color-burn | hard-light |
           soft-light | difference | exclusion | hue | saturation |
           color | luminosity


http://blogs.adobe.com/webplatform/2013/01/28/blending-features-in-canvas/

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var mountains;
	var bricks;
	
	function preload() {
	  mountains = loadImage("assets/rockies.jpg");
	  bricks = loadImage("assets/bricks_third.jpg");
	}
	
	function setup() {
	  mountains.blend(bricks, 0, 0, 33, 100, 67, 0, 33, 100, ADD);
	  image(mountains, 0, 0);
	  image(bricks, 0, 0);
	}
	var mountains;
	var bricks;
	
	function preload() {
	  mountains = loadImage("assets/rockies.jpg");
	  bricks = loadImage("assets/bricks_third.jpg");
	}
	
	function setup() {
	  mountains.blend(bricks, 0, 0, 33, 100, 67, 0, 33, 100, DARKEST);
	  image(mountains, 0, 0);
	  image(bricks, 0, 0);
	}
	var mountains;
	var bricks;
	
	function preload() {
	  mountains = loadImage("assets/rockies.jpg");
	  bricks = loadImage("assets/bricks_third.jpg");
	}
	
	function setup() {
	  mountains.blend(bricks, 0, 0, 33, 100, 67, 0, 33, 100, LIGHTEST);
	  image(mountains, 0, 0);
	  image(bricks, 0, 0);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
