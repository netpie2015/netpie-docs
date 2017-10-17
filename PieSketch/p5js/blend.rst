.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

blend()
=======

คัดลอกพื้นที่พิกเซลจากภาพหนึ่งไปยังอีกภาพหนึ่งโดยใช้โหมดผสมผสานที่ระบุเพื่อดำเนินการ 
โหมดการผสมผสานที่ใช้ได้คือ: BLEND | DARKEST | LIGHTEST | ความแตกต่าง | ทวีคูณ | การยกเว้น | หน้าจอ | แทนที่ | OVERLAY | HARD_LIGHT | SOFT_LIGHT | DODGE | เบิร์น | เพิ่ม | ปกติ

.. Copies a region of pixels from one image to another, using a specified
.. blend mode to do the operation.
.. 
.. Available blend modes are: BLEND | DARKEST | LIGHTEST | DIFFERENCE |
.. MULTIPLY| EXCLUSION | SCREEN | REPLACE | OVERLAY | HARD_LIGHT |
.. SOFT_LIGHT | DODGE | BURN | ADD | NORMAL

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

- ``blendMode``  Integer: โหมดผสมผสาน

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

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var img0;
	var img1;
	
	function preload() {
	  img0 = loadImage("assets/rockies.jpg");
	  img1 = loadImage("assets/bricks_third.jpg");
	}
	
	function setup() {
	  background(img0);
	  image(img1, 0, 0);
	  blend(img1, 0, 0, 33, 100, 67, 0, 33, 100, LIGHTEST);
	}
	var img0;
	var img1;
	
	function preload() {
	  img0 = loadImage("assets/rockies.jpg");
	  img1 = loadImage("assets/bricks_third.jpg");
	}
	
	function setup() {
	  background(img0);
	  image(img1, 0, 0);
	  blend(img1, 0, 0, 33, 100, 67, 0, 33, 100, DARKEST);
	}
	var img0;
	var img1;
	
	function preload() {
	  img0 = loadImage("assets/rockies.jpg");
	  img1 = loadImage("assets/bricks_third.jpg");
	}
	
	function setup() {
	  background(img0);
	  image(img1, 0, 0);
	  blend(img1, 0, 0, 33, 100, 67, 0, 33, 100, ADD);
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
