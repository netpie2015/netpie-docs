.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

keyTyped()
==========

ฟังก์ชัน keyTyped () เรียกว่าทุกครั้งที่มีการกดปุ่ม แต่ปุ่มดำเนินการเช่น Ctrl, Shift และ Alt จะถูกละเลย กดคีย์ล่าสุดจะถูกเก็บไว้ในตัวแปรหลัก 
เนื่องจากระบบปฏิบัติการจัดการกับการทำซ้ำที่สำคัญการกดคีย์ค้างไว้จะทำให้หลาย ๆ การเรียกไปยัง keyTyped () (และ keyReleased () ด้วย) อัตราการทำซ้ำถูกกำหนดโดยระบบปฏิบัติการและวิธีการกำหนดค่าคอมพิวเตอร์แต่ละเครื่อง 
เบราว์เซอร์อาจมีพฤติกรรมเริ่มต้นต่างกันไปตามเหตุการณ์สำคัญต่างๆ หากต้องการป้องกันไม่ให้เกิดการทำงานดีฟอลต์สำหรับเหตุการณ์นี้ให้เพิ่ม &quot;return false&quot; ที่ด้านท้ายสุดของเมธอด

.. The keyTyped() function is called once every time a key is pressed, but
.. action keys such as Ctrl, Shift, and Alt are ignored. The most recent
.. key pressed will be stored in the key variable.
.. 
.. Because of how operating systems handle key repeats, holding down a key
.. will cause multiple calls to keyTyped() (and keyReleased() as well). The
.. rate of repeat is set by the operating system and how each computer is
.. configured.
.. 
.. Browsers may have different default behaviors attached to various key
.. events. To prevent any default behavior for this event, add "return false"
.. to the end of the method.
**รูปแบบการใช้งาน**

keyTyped ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var value = 0;
	function draw() {
	  fill(value);
	  rect(25, 25, 50, 50);
	}
	function keyTyped() {
	  if (key === 'a') {
	    value = 255;
	  } else if (key === 'b') {
	    value = 0;
	  }
	  // uncomment to prevent any default behavior
	  // return false;
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
