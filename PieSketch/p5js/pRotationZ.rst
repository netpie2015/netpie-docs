.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

pRotationZ
============

ตัวแปรระบบ pRotationZ ประกอบด้วยการหมุนของอุปกรณ์พร้อมแกน z ในกรอบก่อนหน้ากรอบปัจจุบัน ค่าจะแสดงเป็น 0 ถึง 359 องศา 
pRotationZ สามารถใช้กับ rotationZ เพื่อกำหนดทิศทางการหมุนของอุปกรณ์ตามแนวแกน Z

.. The system variable pRotationZ always contains the rotation of the
.. device along the z axis in the frame previous to the current frame. Value
.. is represented as 0 to 359 degrees.
.. 
.. pRotationZ can also be used with rotationZ to determine the rotate
.. direction of the device along the Z-axis.

**รูปแบบการใช้งาน**

pRotationZ

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// A simple if statement looking at whether
	// rotationZ - pRotationZ < 0 is true or not will be
	// sufficient for determining the rotate direction
	// in most cases.
	
	// Some extra logic is needed to account for cases where
	// the angles wrap around.
	var rotateDirection = 'clockwise';
	
	if ((rotationZ - pRotationZ > 0 &&
	  rotationZ - pRotationZ < 270)||
	  rotationZ - pRotationZ < -270){
	
	  rotateDirection = 'clockwise';
	
	} else if (rotationZ - pRotationZ < 0 ||
	  rotationZ - pRotationZ > 270){
	
	  rotateDirection = 'counter-clockwise';
	
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
