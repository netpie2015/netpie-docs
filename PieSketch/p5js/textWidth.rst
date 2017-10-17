.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

textWidth()
===========

คำนวณและส่งกลับค่าความกว้างของอักขระหรือสตริงข้อความ

.. Calculates and returns the width of any character or text string.

**รูปแบบการใช้งาน**

textWidth ( theText )

**พารามิเตอร์**

- ``theText``  String: สายอักขระที่จะวัด

.. ``theText``  String: the String of characters to measure

**ค่าที่ส่งออกมา**

- Number: 

.. Number: 

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	textSize(28);
	
	var aChar = 'P';
	var cWidth = textWidth(aChar);
	text(aChar, 0, 40);
	line(cWidth, 0, cWidth, 50);
	
	var aString = "p5.js";
	var sWidth = textWidth(aString);
	text(aString, 0, 85);
	line(sWidth, 50, sWidth, 100);

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
