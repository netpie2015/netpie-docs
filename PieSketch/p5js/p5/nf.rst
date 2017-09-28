.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

nf()
====

ฟังก์ชันยูทิลิตี้สำหรับการจัดรูปแบบตัวเลขเป็นสตริง มีสองเวอร์ชัน: หนึ่งสำหรับการฟอร์แมตลอยตัวและสำหรับการจัดรูปแบบ ints ค่าสำหรับตัวเลขซ้ายและขวาควรเป็นจำนวนเต็มบวก

.. Utility function for formatting numbers into strings. There are two
.. versions: one for formatting floats, and one for formatting ints.
.. The values for the digits, left, and right parameters should always
.. be positive integers.

**รูปแบบการใช้งาน**

nf ( num, [left], [right] )

**พารามิเตอร์**

- ``num``  Number,String: หมายเลขเพื่อจัดรูปแบบ

- ``left``  Number,String: จำนวนหลักที่อยู่ทางซ้ายของจุดทศนิยม

- ``right``  Number,String: จำนวนหลักที่อยู่ทางขวาของจุดทศนิยม

.. ``num``  Number,String: the Number to format
.. ``left``  Number,String: number of digits to the left of the decimal point
.. ``right``  Number,String: number of digits to the right of the decimal point

**ค่าที่ส่งออกมา**

- String: รูปแบบสตริง

.. String: formatted String

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
