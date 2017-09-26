.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

nfc()
=====

ฟังก์ชันยูทิลิตี้สำหรับการจัดรูปแบบตัวเลขลงในสตริงและวางเครื่องหมายจุลภาคที่เหมาะสมเพื่อทำเครื่องหมายหน่วยของ 1000 มีสองเวอร์ชัน: หนึ่งสำหรับการจัดรูปแบบ ints และอีกอันหนึ่งสำหรับจัดรูปแบบอาร์เรย์ของ ints ค่าสำหรับพารามิเตอร์ที่ถูกต้องควรเป็นจำนวนเต็มบวก

.. Utility function for formatting numbers into strings and placing
.. appropriate commas to mark units of 1000. There are two versions: one
.. for formatting ints, and one for formatting an array of ints. The value
.. for the right parameter should always be a positive integer.
**รูปแบบการใช้งาน**

nfc ( num, [right] )

**พารามิเตอร์**

- ``num``  Number,String: หมายเลขเพื่อจัดรูปแบบ

- ``right``  Number,String: จำนวนหลักที่อยู่ทางขวาของจุดทศนิยม

.. ``num``  Number,String: the Number to format
.. ``right``  Number,String: number of digits to the right of the
                                 decimal point

**ค่าที่ส่งออกมา**

- String: รูปแบบสตริง

.. String: formatted String

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
