.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

byte()
======

แปลงหมายเลขสตริงหรือ boolean เป็นตัวแทนไบต์ ไบต์สามารถมีได้เพียงจำนวนเต็มระหว่าง -128 ถึง 127 ดังนั้นเมื่อมีการแปลงค่าภายนอกช่วงนี้จะมีการรวมเอาไบต์ไว้ เมื่ออาร์เรย์ของค่าตัวเลขสตริงหรือแบบบูลถูกส่งผ่านไประบบจะส่งคืนอาร์เรย์ของไบต์ที่มีความยาวเท่ากัน

.. Converts a number, string or boolean to its byte representation.
.. A byte can be only a whole number between -128 and 127, so when a value
.. outside of this range is converted, it wraps around to the corresponding
.. byte representation. When an array of number, string or boolean values is
.. passed in, then an array of bytes the same length is returned.
**รูปแบบการใช้งาน**

byte ( n )

**พารามิเตอร์**

- ``n``  String,Boolean,Number: ค่าเพื่อแยกวิเคราะห์

.. ``n``  String,Boolean,Number: value to parse

**ค่าที่ส่งออกมา**

- Number: การแสดงค่าไบต์

.. Number: byte representation of value

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
