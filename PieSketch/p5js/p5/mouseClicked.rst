.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

mouseClicked()
==============

ฟังก์ชัน mouseClicked () เรียกว่าครั้งหลังจากที่กดปุ่มเมาส์แล้วปล่อยออกมา 
เบราว์เซอร์จัดการการคลิกที่แตกต่างกันดังนั้นฟังก์ชันนี้จึงรับประกันได้ว่าจะทำงานเมื่อคลิกปุ่มเมาส์ซ้ายเท่านั้น เมื่อต้องการจัดการกับปุ่มเมาส์อื่น ๆ ที่ถูกกดหรือปล่อยให้ดูที่ mousePressed () หรือ mouseReleased () 
เบราว์เซอร์อาจมีพฤติกรรมเริ่มต้นแตกต่างกันไปตามเหตุการณ์ต่างๆของเมาส์ หากต้องการป้องกันไม่ให้เกิดการทำงานดีฟอลต์สำหรับเหตุการณ์นี้ให้เพิ่ม &quot;return false&quot; ที่ด้านท้ายสุดของเมธอด

.. The mouseClicked() function is called once after a mouse button has been
.. pressed and then released.
.. 
.. Browsers handle clicks differently, so this function is only guaranteed to be
.. run when the left mouse button is clicked. To handle other mouse buttons
.. being pressed or released, see mousePressed() or mouseReleased().
.. 
.. Browsers may have different default
.. behaviors attached to various mouse events. To prevent any default
.. behavior for this event, add "return false" to the end of the method.
**รูปแบบการใช้งาน**

mouseClicked ( )

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
	
	function mouseClicked() {
	  if (value == 0) {
	    value = 255;
	  } else {
	    value = 0;
	  }
	}

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	function mouseClicked() {
	  ellipse(mouseX, mouseY, 5, 5);
	  // prevent default
	  return false;
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
