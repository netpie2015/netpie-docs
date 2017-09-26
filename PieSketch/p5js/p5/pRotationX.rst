.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

pRotationX
============

ตัวแปรระบบ pRotationX ประกอบด้วยการหมุนของอุปกรณ์ตามแนวแกน x ในกรอบก่อนหน้ากรอบปัจจุบัน ค่าจะแสดงเป็น 0 ถึง +/- 180 องศา 
pRotationX สามารถใช้กับ rotationX เพื่อกำหนดทิศทางการหมุนของอุปกรณ์ตามแนวแกน X

.. The system variable pRotationX always contains the rotation of the
.. device along the x axis in the frame previous to the current frame. Value
.. is represented as 0 to +/-180 degrees.
.. 
.. pRotationX can also be used with rotationX to determine the rotate
.. direction of the device along the X-axis.

**รูปแบบการใช้งาน**

pRotationX

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// A simple if statement looking at whether
	// rotationX - pRotationX < 0 is true or not will be
	// sufficient for determining the rotate direction
	// in most cases.
	
	// Some extra logic is needed to account for cases where
	// the angles wrap around.
	var rotateDirection = 'clockwise';
	
	// Simple range conversion to make things simpler.
	// This is not absolutely neccessary but the logic
	// will be different in that case.
	
	var rX = rotationX + 180;
	var pRX = pRotationX + 180;
	
	if ((rX - pRX > 0 && rX - pRX < 270)|| rX - pRX < -270){
	  rotateDirection = 'clockwise';
	} else if (rX - pRX < 0 || rX - pRX > 270){
	  rotateDirection = 'counter-clockwise';
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
