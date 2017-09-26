.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

nfs()
=====

ฟังก์ชันยูทิลิตี้สำหรับการจัดรูปแบบตัวเลขเป็นสตริง คล้ายกับ nf () แต่ทำให้ &quot;&quot; (ช่องว่าง) อยู่ข้างหน้าตัวเลขบวกและ &quot;-&quot; อยู่ด้านหน้าของตัวเลขลบ มีสองเวอร์ชัน: หนึ่งสำหรับการฟอร์แมตลอยตัวและสำหรับการจัดรูปแบบ ints ค่าสำหรับตัวเลขซ้ายและขวาควรเป็นจำนวนเต็มบวก

.. Utility function for formatting numbers into strings. Similar to nf() but
.. puts a " " (space) in front of positive numbers and a "-" in front of
.. negative numbers. There are two versions: one for formatting floats, and
.. one for formatting ints. The values for the digits, left, and right
.. parameters should always be positive integers.

**รูปแบบการใช้งาน**

nfs ( num, [left], [right] )

**พารามิเตอร์**

- ``num``  Number: หมายเลขเพื่อจัดรูปแบบ

- ``left``  Number: จำนวนหลักที่อยู่ทางซ้ายของจุดทศนิยม

- ``right``  Number: จำนวนหลักที่อยู่ทางขวาของจุดทศนิยม

.. ``num``  Number: the Number to format
.. ``left``  Number: number of digits to the left of the decimal point
.. ``right``  Number: number of digits to the right of the decimal point

**ค่าที่ส่งออกมา**

- String: รูปแบบสตริง

.. String: formatted String

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
