.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

hex()
=====

แปลงหมายเลขเป็นสตริงในสัญกรณ์เลขฐานสิบหกที่เท่ากัน ถ้าพารามิเตอร์ที่สองถูกส่งมาจะใช้เพื่อกำหนดจำนวนอักขระที่จะสร้างในสัญกรณ์เลขฐานสิบหก เมื่ออาร์เรย์ถูกส่งผ่านไปอาร์เรย์ของสตริงในสัญกรณ์เลขฐานสิบหกที่มีความยาวเท่ากันจะถูกส่งกลับ

.. Converts a number to a string in its equivalent hexadecimal notation. If a
.. second parameter is passed, it is used to set the number of characters to
.. generate in the hexadecimal notation. When an array is passed in, an
.. array of strings in hexadecimal notation of the same length is returned.

**รูปแบบการใช้งาน**

hex ( n, [digits] )

**พารามิเตอร์**

- ``n``  Number: ค่าเพื่อแยกวิเคราะห์

- ``digits``  Number: 

.. ``n``  Number: value to parse
.. ``digits``  Number: 

**ค่าที่ส่งออกมา**

- String: การแทนสตริงเลขฐานสิบหก

.. String: hexadecimal string representation of value

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
