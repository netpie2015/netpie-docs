.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

touchMoved()
============

ฟังก์ชัน touchMoved () เรียกว่าทุกครั้งที่มีการบันทึกการแตะย้าย ถ้าไม่มีฟังก์ชัน touchMoved () ฟังก์ชัน mouseDragged () จะถูกเรียกใช้แทนถ้ากำหนดไว้ 
เบราว์เซอร์อาจมีพฤติกรรมเริ่มต้นแตกต่างกันไปตามเหตุการณ์การสัมผัสต่างๆ หากต้องการป้องกันไม่ให้เกิดการทำงานดีฟอลต์สำหรับเหตุการณ์นี้ให้เพิ่ม "return false" ที่ด้านท้ายสุดของเมธอด

.. The touchMoved() function is called every time a touch move is registered.
.. If no touchMoved() function is defined, the mouseDragged() function will
.. be called instead if it is defined.
.. 
.. Browsers may have different default behaviors attached to various touch
.. events. To prevent any default behavior for this event, add "return false"
.. to the end of the method.

**รูปแบบการใช้งาน**

touchMoved ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Move your finger across the page
	// to change its value
	
	var value = 0;
	function draw() {
	  fill(value);
	  rect(25, 25, 50, 50);
	}
	function touchMoved() {
	  value = value + 5;
	  if (value > 255) {
	    value = 0;
	  }
	}

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	function touchMoved() {
	  ellipse(mouseX, mouseY, 5, 5);
	  // prevent default
	  return false;
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
