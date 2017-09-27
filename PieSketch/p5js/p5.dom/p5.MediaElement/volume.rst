.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

volume()
========

ตั้งค่าปริมาณสำหรับองค์ประกอบสื่อ HTML5 ถ้าไม่ได้รับอาร์กิวเมนต์ให้ส่งคืนไดรฟ์ข้อมูลปัจจุบัน

.. Sets volume for this HTML5 media element. If no argument is given,
.. returns the current volume.

**รูปแบบการใช้งาน**

volume ( [val] )

**พารามิเตอร์**

- ``val``  Number: ระหว่าง 0.0 ถึง 1.0

.. ``val``  Number: volume between 0.0 and 1.0

**ค่าที่ส่งออกมา**

- Number,p5.MediaElement: ปัจจุบันหรือ p5.MediaElement

.. Number,p5.MediaElement: current volume or p5.MediaElement

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
