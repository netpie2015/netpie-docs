.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

cone()
======

วาดกรวยด้วยรัศมีและความสูงที่กำหนด

.. Draw a cone with given radius and height

**รูปแบบการใช้งาน**

cone ( radius, height, [detailX], [detailY] )

**พารามิเตอร์**

- ``radius``  Number: รัศมีของพื้นผิวด้านล่าง

- ``height``  Number: ความสูงของกรวย

- ``detailX``  Number: ไม่จำเป็น: จำนวนกลุ่มส่วนที่มากขึ้นค่าเริ่มต้นของเรขาคณิตที่ราบรื่นคือ 24

- ``detailY``  Number: ไม่จำเป็น: จำนวนกลุ่มส่วนที่มากขึ้นค่าเริ่มต้นของเรขาคณิตที่ราบรื่นคือ 16

.. ``radius``  Number: radius of the bottom surface
.. ``height``  Number: height of the cone
.. ``detailX``  Number: optional: number of segments, the more segments the smoother geometry default is 24
.. ``detailY``  Number: optional: number of segments, the more segments the smoother geometry default is 16

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	//draw a spinning cone with radius 200 and height 200
	function setup(){
	  createCanvas(100, 100, WEBGL);
	}
	
	function draw(){
	  background(200);
	  rotateX(frameCount * 0.01);
	  rotateZ(frameCount * 0.01);
	  cone(200, 200);
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
