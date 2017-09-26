.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

torus()
=======

วาดพรูด้วยรัศมีและรัศมีของรัศมี

.. Draw a torus with given radius and tube radius

**รูปแบบการใช้งาน**

torus ( radius, tubeRadius, [detailX], [detailY] )

**พารามิเตอร์**

- ``radius``  Number: รัศมีของทั้งวง

- ``tubeRadius``  Number: รัศมีของหลอด

- ``detailX``  Number: ไม่จำเป็น: จำนวนเซ็กเมนต์ในมิติ x ส่วนที่มากขึ้นเรขาคณิตที่ราบรื่นมากขึ้นคือ 24

- ``detailY``  Number: ไม่จำเป็น: จำนวนเซ็กเมนต์ใน y-dimension ส่วนที่มากขึ้นค่าเริ่มต้นของเรขาคณิตที่ราบรื่นคือ 16

.. ``radius``  Number: radius of the whole ring
.. ``tubeRadius``  Number: radius of the tube
.. ``detailX``  Number: optional: number of segments in x-dimension, the more segments the smoother geometry default is 24
.. ``detailY``  Number: optional: number of segments in y-dimension, the more segments the smoother geometry default is 16

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	//draw a spinning torus with radius 200 and tube radius 60
	function setup(){
	  createCanvas(100, 100, WEBGL);
	}
	
	function draw(){
	  background(200);
	  rotateX(frameCount * 0.01);
	  rotateY(frameCount * 0.01);
	  torus(200, 60);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
