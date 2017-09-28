.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

angleMode()
===========

ตั้งค่าโหมดปัจจุบันของ p5 ไปยังโหมดที่กำหนด โหมดค่าเริ่มต้นคือ RADIANS

.. Sets the current mode of p5 to given mode. Default mode is RADIANS.

**รูปแบบการใช้งาน**

angleMode ( mode )

**พารามิเตอร์**

- ``mode``  Constant: ทั้ง RADIANS หรือ DEGREES

.. ``mode``  Constant: either RADIANS or DEGREES

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function draw(){
	  background(204);
	  angleMode(DEGREES); // Change the mode to DEGREES
	  var a = atan2(mouseY-height/2, mouseX-width/2);
	  translate(width/2, height/2);
	  push();
	  rotate(a);
	  rect(-20, -5, 40, 10); // Larger rectangle is rotating in degrees
	  pop();
	  angleMode(RADIANS); // Change the mode to RADIANS
	  rotate(a); // var a stays the same
	  rect(-40, -5, 20, 10); // Smaller rectangle is rotating in radians
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
