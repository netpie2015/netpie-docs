.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

touchEnded()
============

ฟังก์ชัน touchEnded () เรียกว่าทุกครั้งที่มีการแตะ หากไม่มีการกำหนดฟังก์ชัน touchEnded () ฟังก์ชัน mouseReleased () จะถูกเรียกใช้แทนถ้ากำหนดไว้ 
เบราว์เซอร์อาจมีพฤติกรรมเริ่มต้นแตกต่างกันไปตามเหตุการณ์การสัมผัสต่างๆ หากต้องการป้องกันไม่ให้เกิดการทำงานดีฟอลต์สำหรับเหตุการณ์นี้ให้เพิ่ม "return false" ที่ด้านท้ายสุดของเมธอด

.. The touchEnded() function is called every time a touch ends. If no
.. touchEnded() function is defined, the mouseReleased() function will be
.. called instead if it is defined.
.. 
.. Browsers may have different default behaviors attached to various touch
.. events. To prevent any default behavior for this event, add "return false"
.. to the end of the method.

**รูปแบบการใช้งาน**

touchEnded ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Release touch within the image to
	// change the value of the rectangle
	
	var value = 0;
	function draw() {
	  fill(value);
	  rect(25, 25, 50, 50);
	}
	function touchEnded() {
	  if (value == 0) {
	    value = 255;
	  } else {
	    value = 0;
	  }
	}

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	function touchEnded() {
	  ellipse(mouseX, mouseY, 5, 5);
	  // prevent default
	  return false;
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
