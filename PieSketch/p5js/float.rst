.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

float()
=======

แปลงสายอักขระให้เป็นค่าแทน floating point เนื้อหาของสตริงต้องเหมือนกับตัวเลขหรือ NaN (ไม่ใช่ตัวเลข) จะถูกส่งกลับ ยกตัวอย่างเช่น float ("1234.56") จะประเมินเป็น 1234.56 แต่ float ("giraffe") จะกลับ NaN เมื่ออาร์เรย์ของค่าถูกส่งผ่านไปแล้วอาร์เรย์ของ floats ที่มีความยาวเท่ากันจะถูกส่งกลับ

.. Converts a string to its floating point representation. The contents of a
.. string must resemble a number, or NaN (not a number) will be returned.
.. For example, float("1234.56") evaluates to 1234.56, but float("giraffe")
.. will return NaN.
.. When an array of values is passed in, then an array of floats of the same
.. length is returned.

**รูปแบบการใช้งาน**

float ( str )

**พารามิเตอร์**

- ``str``  String: สตริงแบบลอยเพื่อแยกวิเคราะห์

.. ``str``  String: float string to parse

**ค่าที่ส่งออกมา**

- Number: แสดงจุดลอยตัวของสตริง

.. Number: floating point representation of string

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var str = '20';
	var diameter = float(str);
	ellipse(width/2, height/2, diameter, diameter);

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
