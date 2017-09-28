.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

mouseReleased()
===============

ฟังก์ชัน mouseReleased () เรียกว่าทุกครั้งที่มีการปล่อยปุ่มเมาส์ หากไม่มีฟังก์ชัน mouseReleased () ฟังก์ชัน touchEnded () จะถูกเรียกใช้แทนถ้ากำหนดไว้ 
เบราว์เซอร์อาจมีพฤติกรรมเริ่มต้นแตกต่างกันไปตามเหตุการณ์ต่างๆของเมาส์ หากต้องการป้องกันไม่ให้เกิดการทำงานดีฟอลต์สำหรับเหตุการณ์นี้ให้เพิ่ม "return false" ที่ด้านท้ายสุดของเมธอด

.. The mouseReleased() function is called every time a mouse button is
.. released. If no mouseReleased() function is defined, the touchEnded()
.. function will be called instead if it is defined.
.. 
.. Browsers may have different default
.. behaviors attached to various mouse events. To prevent any default
.. behavior for this event, add "return false" to the end of the method.

**รูปแบบการใช้งาน**

mouseReleased ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Click within the image to change
	// the value of the rectangle
	// after the mouse has been clicked
	
	var value = 0;
	function draw() {
	  fill(value);
	  rect(25, 25, 50, 50);
	}
	function mouseReleased() {
	  if (value == 0) {
	    value = 255;
	  } else {
	    value = 0;
	  }
	}

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	function mouseReleased() {
	  ellipse(mouseX, mouseY, 5, 5);
	  // prevent default
	  return false;
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
