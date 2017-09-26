.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

millis()
========

ส่งกลับจำนวนมิลลิวินาที (พันหนึ่งวินาที) ตั้งแต่เริ่มต้นโปรแกรม ข้อมูลนี้มักใช้สำหรับเหตุการณ์การจับเวลาและลำดับภาพเคลื่อนไหว

.. Returns the number of milliseconds (thousandths of a second) since
.. starting the program. This information is often used for timing events and
.. animation sequences.

**รูปแบบการใช้งาน**

millis ( )

**ค่าที่ส่งออกมา**

- Number: จำนวนมิลลิวินาทีตั้งแต่เริ่มต้นโปรแกรม

.. Number: the number of milliseconds since starting the program

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var millisecond = millis();
	text("Milliseconds \nrunning: \n" + millisecond, 5, 40);

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
