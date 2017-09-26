.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

mousePressed()
==============

ฟังก์ชัน mousePressed () เรียกว่าครั้งหลังจากทุกครั้งที่กดปุ่มเมาส์ ตัวแปร mouseButton (ดูรายการอ้างอิงที่เกี่ยวข้อง) สามารถใช้เพื่อกำหนดว่าปุ่มใดถูกกด หากไม่มีฟังก์ชัน mousePressed () ฟังก์ชัน touchStarted () จะถูกเรียกใช้แทนถ้ากำหนดไว้ 
เบราว์เซอร์อาจมีพฤติกรรมเริ่มต้นแตกต่างกันไปตามเหตุการณ์ต่างๆของเมาส์ หากต้องการป้องกันไม่ให้เกิดการทำงานดีฟอลต์สำหรับเหตุการณ์นี้ให้เพิ่ม &quot;return false&quot; ที่ด้านท้ายสุดของเมธอด

.. The mousePressed() function is called once after every time a mouse button
.. is pressed. The mouseButton variable (see the related reference entry)
.. can be used to determine which button has been pressed. If no
.. mousePressed() function is defined, the touchStarted() function will be
.. called instead if it is defined.
.. 
.. Browsers may have different default
.. behaviors attached to various mouse events. To prevent any default
.. behavior for this event, add "return false" to the end of the method.

**รูปแบบการใช้งาน**

mousePressed ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Click within the image to change
	// the value of the rectangle
	
	var value = 0;
	function draw() {
	  fill(value);
	  rect(25, 25, 50, 50);
	}
	function mousePressed() {
	  if (value == 0) {
	    value = 255;
	  } else {
	    value = 0;
	  }
	}

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	function mousePressed() {
	  ellipse(mouseX, mouseY, 5, 5);
	  // prevent default
	  return false;
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
