.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

apply()
=======

ใช้ฟังก์ชันตัวกรองกับผืนผ้าใบ ความแตกต่างระหว่างฟังก์ชันการกรองนี้กับฟังก์ชันการกรองตามจริงที่กำหนดไว้ด้านล่างนี้คือการทำงานของตัวกรองโดยทั่วไปจะปรับเปลี่ยนบัฟเฟอร์ของพิกเซล แต่ไม่ได้นำข้อมูลดังกล่าวกลับไปใช้ผืนผ้าใบ (ซึ่งจะปรับปรุงสิ่งที่มองเห็นได้จริง) ตรงกันข้ามวิธีนี้จะทำให้การเปลี่ยนแปลงที่มองเห็นได้จริงในผืนผ้าใบ วิธีการสมัครเป็นวิธีที่ผู้เรียกร้องของโมดูลนี้ใช้กันโดยทั่วไป ได้รับการแยกออกจากตัวกรองจริงเพื่อสนับสนุนกรณีการใช้งานขั้นสูงในการสร้างห่วงโซ่กรองที่ดำเนินการโดยไม่ต้องอัปเดตผืนผ้าใบในระหว่าง everystep

.. Applys a filter function to a canvas.
.. The difference between this and the actual filter functions defined below
.. is that the filter functions generally modify the pixel buffer but do
.. not actually put that data back to the canvas (where it would actually
.. update what is visible). By contrast this method does make the changes
.. actually visible in the canvas.
.. The apply method is the method that callers of this module would generally
.. use. It has been separated from the actual filters to support an advanced
.. use case of creating a filter chain that executes without actually updating
.. the canvas in between everystep.
**รูปแบบการใช้งาน**

apply ( canvas, func, filterParam )

**พารามิเตอร์**

- ``canvas``  HTMLCanvasElement: [รายละเอียด]

- ``func``  function: [รายละเอียด]

- ``filterParam``  Object: [รายละเอียด]

.. ``canvas``  HTMLCanvasElement: [description]
.. ``func``  function: [description]
.. ``filterParam``  Object: [description]

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
