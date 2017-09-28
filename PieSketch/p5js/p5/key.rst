.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

key
=====

คีย์ตัวแปรระบบประกอบด้วยค่าของคีย์ล่าสุดบนแป้นพิมพ์ที่พิมพ์อยู่เสมอ เพื่อให้ได้ตัวพิมพ์ใหญ่ที่เหมาะสมคุณควรใช้คีย์นี้ภายในคีย์ไทม์ () สำหรับคีย์ที่ไม่ใช่ ASCII ให้ใช้ตัวแปร keyCode

.. The system variable key always contains the value of the most recent
.. key on the keyboard that was typed. To get the proper capitalization, it
.. is best to use it within keyTyped(). For non-ASCII keys, use the keyCode
.. variable.

**รูปแบบการใช้งาน**

key

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Click any key to display it!
	// (Not Guaranteed to be Case Sensitive)
	function setup() {
	  fill(245, 123, 158);
	  textSize(50);
	}
	
	function draw() {
	  background(200);
	  text(key, 33,65); // Display last key pressed.
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
