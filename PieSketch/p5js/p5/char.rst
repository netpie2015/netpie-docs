.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

char()
======

แปลงหมายเลขหรือสตริงเป็นอักขระสตริงอักขระเดียวที่สอดคล้องกัน หากมีการระบุพารามิเตอร์สตริงจะมีการแยกวิเคราะห์เป็นจำนวนเต็มเป็นครั้งแรกและแปลเป็นสตริงอักขระเดียว เมื่ออาร์เรย์ของตัวเลขหรือค่าสตริงถูกส่งผ่านไประบบจะส่งคืนอาร์เรย์ของสตริงอักขระเดียวที่มีความยาวเท่ากัน

.. Converts a number or string to its corresponding single-character
.. string representation. If a string parameter is provided, it is first
.. parsed as an integer and then translated into a single-character string.
.. When an array of number or string values is passed in, then an array of
.. single-character strings of the same length is returned.
**รูปแบบการใช้งาน**

char ( n )

**พารามิเตอร์**

- ``n``  String,Number: ค่าเพื่อแยกวิเคราะห์

.. ``n``  String,Number: value to parse

**ค่าที่ส่งออกมา**

- String: การแสดงค่าของสายอักขระ

.. String: string representation of value

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
