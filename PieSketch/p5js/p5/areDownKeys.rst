.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

areDownKeys()
=============

ฟังก์ชัน checkDownKeys ส่งกลับค่าบูลีนจริงถ้ากดปุ่มใด ๆ และเป็นเท็จหากไม่มีการกดปุ่มใด ๆ ช่วยหลีกเลี่ยงกรณีที่มีการกดปุ่มหลายปุ่มพร้อมกันและปล่อยคีย์เดียวจากนั้นจะเปลี่ยนคุณสมบัติ keyIsPressed เป็น true

.. The checkDownKeys function returns a boolean true if any keys pressed
.. and a false if no keys are currently pressed.
.. Helps avoid instances where a multiple keys are pressed simultaneously and
.. releasing a single key will then switch the
.. keyIsPressed property to true.
**รูปแบบการใช้งาน**

areDownKeys ( )

**พารามิเตอร์**


.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
