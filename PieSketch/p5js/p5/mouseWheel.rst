.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

mouseWheel()
============

เมาส์ฟังก์ชัน (MouseWheel) จะถูกเรียกใช้งานทุกครั้งที่มีการตรวจพบเหตุการณ์ล้อเมาส์แบบแนวตั้งที่ทริกเกอร์โดยล้อเมาส์จริงหรือด้วยทัชแพด 
คุณสมบัติ event.delta จะส่งกลับจำนวนล้อเลื่อนของเมาส์ที่เลื่อนลง ค่านี้สามารถเป็นค่าบวกหรือค่าลบได้ทั้งนี้ขึ้นอยู่กับทิศทางการเลื่อน (ใน OS X ด้วยการเลื่อนแบบ &quot;ธรรมชาติ&quot; การใช้งานจะมีการเปลี่ยนสัญญาณ) 
เบราว์เซอร์อาจมีพฤติกรรมเริ่มต้นแตกต่างกันไปตามเหตุการณ์ต่างๆของเมาส์ หากต้องการป้องกันไม่ให้เกิดการทำงานดีฟอลต์สำหรับเหตุการณ์นี้ให้เพิ่ม &quot;return false&quot; ที่ด้านท้ายสุดของเมธอด 
เนื่องจากปัจจุบันมีการสนับสนุนเหตุการณ์ &quot;wheel&quot; ใน Safari ฟังก์ชันนี้จะทำงานได้ตามปกติเท่านั้นหากมีการ &quot;return false&quot; ในขณะที่ใช้ Safari

.. The function mouseWheel() is executed every time a vertical mouse wheel
.. event is detected either triggered by an actual mouse wheel or by a
.. touchpad.
.. 
.. The event.delta property returns the amount the mouse wheel
.. have scrolled. The values can be positive or negative depending on the
.. scroll direction (on OS X with "natural" scrolling enabled, the signs
.. are inverted).
.. 
.. Browsers may have different default behaviors attached to various
.. mouse events. To prevent any default behavior for this event, add
.. "return false" to the end of the method.
.. 
.. Due to the current support of the "wheel" event on Safari, the function
.. may only work as expected if "return false" is included while using Safari.

**รูปแบบการใช้งาน**

mouseWheel ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var pos = 25;
	
	function draw() {
	  background(237, 34, 93);
	  fill(0);
	  rect(25, pos, 50, 50);
	}
	
	function mouseWheel(event) {
	  print(event.delta);
	  //move the square according to the vertical scroll amount
	  pos += event.delta;
	  //uncomment to block page scrolling
	  //return false;
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
