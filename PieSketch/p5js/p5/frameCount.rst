.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

frameCount
============

ตัวแปรเฟรม frameCount ประกอบด้วยจำนวนเฟรมที่แสดงขึ้นตั้งแต่เริ่มต้นโปรแกรม ภายในการตั้งค่า () ค่าเป็น 0 หลังจากที่ทำซ้ำครั้งแรกของการวาดเป็น 1 ฯลฯ

.. The system variable frameCount contains the number of frames that have
.. been displayed since the program started. Inside setup() the value is 0,
.. after the first iteration of draw it is 1, etc.

**รูปแบบการใช้งาน**

frameCount

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	    function setup() {
	      frameRate(30);
	      textSize(20);
	      textSize(30);
	      textAlign(CENTER);
	    }
	
	    function draw() {
	      background(200);
	      text(frameCount, width/2, height/2);
	    }
	  

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
