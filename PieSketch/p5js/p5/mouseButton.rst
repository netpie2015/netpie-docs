.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

mouseButton
=============

การประมวลผลจะติดตามโดยอัตโนมัติหากกดปุ่มเมาส์และกดปุ่มใด ค่าของ mouseButton ตัวแปรระบบคือ LEFT, RIGHT หรือ CENTER ขึ้นอยู่กับปุ่มใดที่กดปุ่มสุดท้าย คำเตือน: เบราว์เซอร์อื่นอาจติดตาม mouseButton แตกต่างกัน

.. Processing automatically tracks if the mouse button is pressed and which
.. button is pressed. The value of the system variable mouseButton is either
.. LEFT, RIGHT, or CENTER depending on which button was pressed last.
.. Warning: different browsers may track mouseButton differently.

**รูปแบบการใช้งาน**

mouseButton

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function draw() {
	  background(237, 34, 93);
	  fill(0);
	
	  if (mouseIsPressed) {
	    if (mouseButton == LEFT)
	      ellipse(50, 50, 50, 50);
	    if (mouseButton == RIGHT)
	      rect(25, 25, 50, 50);
	    if (mouseButton == CENTER)
	      triangle(23, 75, 50, 20, 78, 75);
	  }
	
	  print(mouseButton);
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
