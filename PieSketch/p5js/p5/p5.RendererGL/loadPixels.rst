.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

loadPixels()
============

โหลดข้อมูลพิกเซลสำหรับผืนผ้าใบนี้เป็นพิกเซล [] โปรดทราบว่า updatePixels () และ set () ไม่ทำงาน การจัดการพิกเซลใด ๆ ต้องทำโดยตรงไปยังอาร์เรย์ของพิกเซล []

.. Loads the pixels data for this canvas into the pixels[] attribute.
.. Note that updatePixels() and set() do not work.
.. Any pixel manipulation must be done directly to the pixels[] array.

**รูปแบบการใช้งาน**

loadPixels ( starting, starting, width, height )

**พารามิเตอร์**

- ``starting``  Number: พิกเซล x ตำแหน่งค่าเริ่มต้นเป็น 0

- ``starting``  Number: พิกเซล y ตำแหน่งค่าเริ่มต้นเป็น 0

- ``width``  Number: ของพิกเซลที่จะโหลดเริ่มต้นในการร่างความกว้าง

- ``height``  Number: ของพิกเซลที่จะโหลดค่าเริ่มต้นในการร่างความสูง

.. ``starting``  Number: pixel x position, defaults to 0
.. ``starting``  Number: pixel y position, defaults to 0
.. ``width``  Number: of pixels to load, defaults to sketch width
.. ``height``  Number: of pixels to load, defaults to sketch height

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
