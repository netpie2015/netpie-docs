.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

split()
=======

ฟังก์ชัน split () จะจับคู่กับ String.split () ซึ่งจะแบ่ง String เป็นชิ้นโดยใช้อักขระหรือสตริงเป็นตัวคั่น พารามิเตอร์ delim ระบุอักขระหรืออักขระที่ทำเครื่องหมายขอบเขตระหว่างแต่ละชิ้น อาร์เรย์สตริง [] จะถูกส่งคืนที่ประกอบด้วยแต่ละส่วน ฟังก์ชัน splitTokens () ทำงานในรูปแบบคล้าย ๆ กันเว้นแต่จะแบ่งเป็นช่วงของอักขระแทนอักขระหรือลำดับที่ระบุ

.. The split() function maps to String.split(), it breaks a String into
.. pieces using a character or string as the delimiter. The delim parameter
.. specifies the character or characters that mark the boundaries between
.. each piece. A String[] array is returned that contains each of the pieces.
.. The splitTokens() function works in a similar fashion, except that it
.. splits using a range of characters instead of a specific character or
.. sequence.

**รูปแบบการใช้งาน**

split ( value, delim )

**พารามิเตอร์**

- ``value``  String: สายที่จะแยก

- ``delim``  String: สายอักขระที่ใช้ในการแยกข้อมูล

.. ``value``  String: the String to be split
.. ``delim``  String: the String used to separate the data

**ค่าที่ส่งออกมา**

- Array.<String>: อาร์เรย์ของสตริง

.. Array.<String>: Array of Strings

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var names = "Pat,Xio,Alex"
	var splitString = split(names, ",");
	text(splitString[0], 5, 30);
	text(splitString[1], 5, 50);
	text(splitString[2], 5, 70);

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
