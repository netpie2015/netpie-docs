.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

keyPressed()
============

ฟังก์ชัน keyPressed () เรียกว่าครั้งทุกครั้งที่กดปุ่ม keyCode สำหรับคีย์ที่ถูกกดถูกเก็บไว้ในตัวแปร keyCode 
สำหรับคีย์ที่ไม่ใช่ ASCII ให้ใช้ตัวแปร keyCode คุณสามารถตรวจสอบได้ว่าคีย์ลัดมีค่าเท่ากับ BACKSPACE, DELETE, ENTER, RETURN, TAB, ESCAPE, SHIFT, CONTROL, OPTION, ALT, UP_ARROW, DOWN_ARROW, LEFT_ARROW, RIGHT_ARROW 
สำหรับคีย์ ASCII ที่ถูกกดจะถูกเก็บไว้ในตัวแปรหลัก อย่างไรก็ตามไม่ได้แยกความแตกต่างระหว่างตัวพิมพ์ใหญ่และตัวพิมพ์เล็ก ด้วยเหตุนี้ขอแนะนำให้ใช้ keyTyped () เพื่ออ่านตัวแปรหลักซึ่งจะแยกแยะกรณีของตัวแปร 
เนื่องจากระบบปฏิบัติการจัดการกับการทำซ้ำที่สำคัญการกดคีย์ค้างไว้อาจทำให้เกิดการเรียกหลาย ๆ ครั้งที่ keyTyped () (และ keyReleased () ด้วย) อัตราการทำซ้ำถูกกำหนดโดยระบบปฏิบัติการและวิธีการกำหนดค่าคอมพิวเตอร์แต่ละเครื่อง 
เบราว์เซอร์อาจมีพฤติกรรมเริ่มต้นต่างกันไปตามเหตุการณ์สำคัญต่างๆ หากต้องการป้องกันไม่ให้เกิดการทำงานดีฟอลต์สำหรับเหตุการณ์นี้ให้เพิ่ม "return false" ที่ด้านท้ายสุดของเมธอด

.. The keyPressed() function is called once every time a key is pressed. The
.. keyCode for the key that was pressed is stored in the keyCode variable.
.. 
.. For non-ASCII keys, use the keyCode variable. You can check if the keyCode
.. equals BACKSPACE, DELETE, ENTER, RETURN, TAB, ESCAPE, SHIFT, CONTROL,
.. OPTION, ALT, UP_ARROW, DOWN_ARROW, LEFT_ARROW, RIGHT_ARROW.
.. 
.. For ASCII keys that was pressed is stored in the key variable. However, it
.. does not distinguish between uppercase and lowercase. For this reason, it
.. is recommended to use keyTyped() to read the key variable, in which the
.. case of the variable will be distinguished.
.. 
.. Because of how operating systems handle key repeats, holding down a key
.. may cause multiple calls to keyTyped() (and keyReleased() as well). The
.. rate of repeat is set by the operating system and how each computer is
.. configured.
.. 
.. Browsers may have different default
.. behaviors attached to various key events. To prevent any default
.. behavior for this event, add "return false" to the end of the method.

**รูปแบบการใช้งาน**

keyPressed ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var value = 0;
	function draw() {
	  fill(value);
	  rect(25, 25, 50, 50);
	}
	function keyPressed() {
	  if (value === 0) {
	    value = 255;
	  } else {
	    value = 0;
	  }
	}

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var value = 0;
	function draw() {
	  fill(value);
	  rect(25, 25, 50, 50);
	}
	function keyPressed() {
	  if (keyCode === LEFT_ARROW) {
	    value = 255;
	  } else if (keyCode === RIGHT_ARROW) {
	    value = 0;
	  }
	}

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function keyPressed(){
	  // Do something
	  return false; // prevent any default behaviour
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
