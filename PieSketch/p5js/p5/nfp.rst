.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

nfp()
=====

ฟังก์ชันยูทิลิตี้สำหรับการจัดรูปแบบตัวเลขเป็นสตริง คล้ายกับ nf () แต่ใส่เครื่องหมาย &quot;+&quot; หน้าตัวเลขบวกและ &quot;-&quot; ไว้ข้างหน้าตัวเลขลบ มีสองเวอร์ชัน: หนึ่งสำหรับการฟอร์แมตลอยตัวและสำหรับการจัดรูปแบบ ints ค่าสำหรับพารามิเตอร์ซ้ายและขวาควรเป็นจำนวนเต็มบวก

.. Utility function for formatting numbers into strings. Similar to nf() but
.. puts a "+" in front of positive numbers and a "-" in front of negative
.. numbers. There are two versions: one for formatting floats, and one for
.. formatting ints. The values for left, and right parameters
.. should always be positive integers.

**รูปแบบการใช้งาน**

nfp ( num, [left], [right] )

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
