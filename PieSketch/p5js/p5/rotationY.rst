.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

rotationY
===========

การหมุนตัวแปรของระบบมักประกอบด้วยการหมุนของอุปกรณ์ตามแนวแกน y ค่าจะแสดงเป็น 0 ถึง +/- 90 องศา 
หมายเหตุ: ลำดับการหมุนเวียนเรียกว่าสำคัญเช่น ถ้าใช้ร่วมกันจะต้องเรียกว่า ZXY ตามลำดับหรืออาจมีพฤติกรรมที่ไม่คาดคิด

.. The system variable rotationY always contains the rotation of the
.. device along the y axis. Value is represented as 0 to +/-90 degrees.
.. 
.. Note: The order the rotations are called is important, ie. if used
.. together, it must be called in the order Z-X-Y or there might be
.. unexpected behaviour.

**รูปแบบการใช้งาน**

rotationY

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup(){
	  createCanvas(100, 100, WEBGL);
	}
	
	function draw(){
	  background(200);
	  //rotateZ(radians(rotationZ));
	  //rotateX(radians(rotationX));
	  rotateY(radians(rotationY));
	  box(200, 200, 200);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
