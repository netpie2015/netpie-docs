.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

lerp()
======

เชิงเส้น interpolate เวกเตอร์ไปยังเวกเตอร์อื่น

.. Linear interpolate the vector to another vector

**รูปแบบการใช้งาน**

lerp ( x, y, z, amt )

**พารามิเตอร์**

- ``x``  p5.Vector: คอมโพเนนต์ x

- ``y``  p5.Vector: องค์ประกอบ y

- ``z``  p5.Vector: ส่วนประกอบ z

- ``amt``  Number: จำนวนของการแก้ไข ค่าระหว่าง 0.0 (เวกเตอร์เก่า) และ 1.0 (เวกเตอร์ใหม่) 0.1 ใกล้กับเวกเตอร์ใหม่ 0.5 อยู่กึ่งกลางระหว่าง

.. ``x``  p5.Vector: the x component
.. ``y``  p5.Vector: the y component
.. ``z``  p5.Vector: the z component
.. ``amt``  Number: the amount of interpolation; some value between 0.0 (old vector) and 1.0 (new vector). 0.1 is very near the new vector. 0.5 is halfway in between.

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
