.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

str()
=====

แปลงสตริงบูลีนสตริงหรือตัวเลขเป็นสตริงแทน เมื่ออาร์เรย์ของค่าถูกส่งผ่านไปแล้วอาร์เรย์ของสตริงที่มีความยาวเท่ากันจะถูกส่งกลับ

.. Converts a boolean, string or number to its string representation.
.. When an array of values is passed in, then an array of strings of the same
.. length is returned.

**รูปแบบการใช้งาน**

str ( n )

**พารามิเตอร์**

- ``n``  String,Boolean,Number,Array: ค่าเพื่อแยกวิเคราะห์

.. ``n``  String,Boolean,Number,Array: value to parse

**ค่าที่ส่งออกมา**

- String: การแสดงค่าของสายอักขระ

.. String: string representation of value

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	print(str("10"));  // "10"
	print(str(10.31)); // "10.31"
	print(str(-10));   // "-10"
	print(str(true));  // "true"
	print(str(false)); // "false"
	print(str([true, "10.3", 9.8])); // [ "true", "10.3", "9.8" ]

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
