.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

textDescent()
=============

ส่งกลับค่าโควต้าของแบบอักษรปัจจุบันที่มีขนาดปัจจุบัน โคตรหมายถึงระยะทางเป็นพิกเซลของตัวละครที่มีระยะห่างที่ยาวที่สุดต่ำกว่าเส้นฐาน

.. Returns the descent of the current font at its current size. The descent
.. represents the distance, in pixels, of the character with the longest
.. descender below the baseline.

**รูปแบบการใช้งาน**

textDescent ( )

**ค่าที่ส่งออกมา**

- Number: 

.. Number: 

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var base = height * 0.75;
	var scalar = 0.8; // Different for each font
	
	textSize(32);  // Set initial text size
	var desc = textDescent() * scalar;  // Calc ascent
	line(0, base+desc, width, base+desc);
	text("dp", 0, base);  // Draw text on baseline
	
	textSize(64);  // Increase text size
	desc = textDescent() * scalar;  // Recalc ascent
	line(40, base + desc, width, base + desc);
	text("dp", 40, base);  // Draw text on baseline

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
