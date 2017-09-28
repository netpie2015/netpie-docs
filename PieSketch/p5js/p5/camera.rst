.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

camera()
========

ตั้งค่าตำแหน่งกล้องสำหรับภาพร่าง 3 มิติ ฟังก์ชันจะทำงานคล้ายคลึงกับ gluLookAt ยกเว้นว่าจะแทนที่เมทริกซ์แบบจำลองที่มีอยู่แทนการใช้การแปลงใด ๆ ที่คำนวณที่นี่ที่ด้านบนของมุมมองแบบจำลองที่มีอยู่ เมื่อเรียกว่าไม่มีอาร์กิวเมนต์ฟังก์ชั่นนี้จะกำหนดค่าเริ่มต้นของกล้องที่เทียบเท่ากับการเรียกกล้องถ่ายรูป (0, 0, (สูง / 2.0) / tan (PI * 30.0 / 180.0), 0, 0, 0, 0, 1, 0);

.. Sets camera position for a 3D sketch. The function behaves similarly
.. gluLookAt, except that it replaces the existing modelview matrix instead
.. of applying any transformations calculated here on top of the existing
.. model view.
.. When called with no arguments, this function
.. sets a default camera equivalent to calling
.. camera(0, 0, (height/2.0) / tan(PI*30.0 / 180.0), 0, 0, 0, 0, 1, 0);

**รูปแบบการใช้งาน**

camera ( [x], [y], [z], [centerX], [centerY], [centerZ], [upX], [upY], [upZ] )

**พารามิเตอร์**

- ``x``  Number: ค่าตำแหน่งกล้องบนแกน x

- ``y``  Number: ค่าตำแหน่งกล้องบนแกน y

- ``z``  Number: ค่าตำแหน่งกล้องบนแกน z

- ``centerX``  Number: พิกัด x แสดงศูนย์กลางของร่าง

- ``centerY``  Number: พิกัด y แทนศูนย์ของร่าง

- ``centerZ``  Number: พิกัด z แสดงศูนย์กลางของร่าง

- ``upX``  Number: องค์ประกอบ x ของทิศทาง &#39;ขึ้น&#39; จากกล้อง

- ``upY``  Number: y ส่วนประกอบของทิศทาง &#39;ขึ้น&#39; จากกล้อง

- ``upZ``  Number: z องค์ประกอบของทิศทาง &#39;ขึ้น&#39; จากกล้อง

.. ``x``  Number: camera position value on x axis
.. ``y``  Number: camera position value on y axis
.. ``z``  Number: camera position value on z axis
.. ``centerX``  Number: x coordinate representing center of the sketch
.. ``centerY``  Number: y coordinate representing center of the sketch
.. ``centerZ``  Number: z coordinate representing center of the sketch
.. ``upX``  Number: x component of direction 'up' from camera
.. ``upY``  Number: y component of direction 'up' from camera
.. ``upZ``  Number: z component of direction 'up' from camera

**ค่าที่ส่งออกมา**

- p5: วัตถุ p5

.. p5: the p5 object

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup(){
	  createCanvas(100, 100, WEBGL);
	}
	function draw(){
	 //move the camera away from the plane by a sin wave
	 camera(0, 0, sin(frameCount * 0.01) * 100, 0, 0, 0, 0, 1, 0);
	 plane(120, 120);
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
