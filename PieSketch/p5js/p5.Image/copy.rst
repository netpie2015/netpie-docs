.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

copy()
======

คัดลอกพื้นที่พิกเซลจากภาพหนึ่งไปยังอีกภาพหนึ่ง ถ้าไม่มี srcImage ระบุไว้ใช้เป็นแหล่งข้อมูล หากแหล่งที่มาและปลายทางมีขนาดไม่เท่ากันจะเป็นการปรับขนาดพิกเซลต้นฉบับให้พอดีกับพื้นที่เป้าหมายที่ระบุ

.. Copies a region of pixels from one image to another. If no
.. srcImage is specified this is used as the source. If the source
.. and destination regions aren't the same size, it will
.. automatically resize source pixels to fit the specified
.. target region.

**รูปแบบการใช้งาน**

copy ( srcImage, sx, sy, sw, sh, dx, dy, dw, dh )

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

.. ``srcImage``  p5.Image,undefined: source image
.. ``sx``  Integer: X coordinate of the source's upper left corner
.. ``sy``  Integer: Y coordinate of the source's upper left corner
.. ``sw``  Integer: source image width
.. ``sh``  Integer: source image height
.. ``dx``  Integer: X coordinate of the destination's upper left corner
.. ``dy``  Integer: Y coordinate of the destination's upper left corner
.. ``dw``  Integer: destination image width
.. ``dh``  Integer: destination image height

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var photo;
	var bricks;
	var x;
	var y;
	
	function preload() {
	  photo = loadImage("assets/rockies.jpg");
	  bricks = loadImage("assets/bricks.jpg");
	}
	
	function setup() {
	  x = bricks.width/2;
	  y = bricks.height/2;
	  photo.copy(bricks, 0, 0, x, y, 0, 0, x, y);
	  image(photo, 0, 0);
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
