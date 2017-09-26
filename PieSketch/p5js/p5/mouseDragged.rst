.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

mouseDragged()
==============

ฟังก์ชัน mouseDragged () เรียกว่าทุกครั้งที่เมาส์เลื่อนและกดปุ่มเมาส์ หากไม่มีการกำหนดฟังก์ชัน mouseDragged () ฟังก์ชัน touchMoved () จะถูกเรียกใช้แทนถ้ากำหนดไว้ 
เบราว์เซอร์อาจมีพฤติกรรมเริ่มต้นแตกต่างกันไปตามเหตุการณ์ต่างๆของเมาส์ หากต้องการป้องกันไม่ให้เกิดการทำงานดีฟอลต์สำหรับเหตุการณ์นี้ให้เพิ่ม &quot;return false&quot; ที่ด้านท้ายสุดของเมธอด

.. The mouseDragged() function is called once every time the mouse moves and
.. a mouse button is pressed. If no mouseDragged() function is defined, the
.. touchMoved() function will be called instead if it is defined.
.. 
.. Browsers may have different default
.. behaviors attached to various mouse events. To prevent any default
.. behavior for this event, add "return false" to the end of the method.

**รูปแบบการใช้งาน**

mouseDragged ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Drag the mouse across the page
	// to change its value
	
	var value = 0;
	function draw() {
	  fill(value);
	  rect(25, 25, 50, 50);
	}
	function mouseDragged() {
	  value = value + 5;
	  if (value > 255) {
	    value = 0;
	  }
	}

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	function mouseDragged() {
	  ellipse(mouseX, mouseY, 5, 5);
	  // prevent default
	  return false;
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
