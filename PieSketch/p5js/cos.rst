.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

cos()
=====

คำนวณโคไซน์ของมุม ฟังก์ชันนี้คำนึงถึงมุมมองปัจจุบัน ค่าจะถูกส่งกลับในช่วง -1 ถึง 1

.. Calculates the cosine of an angle. This function takes into account the
.. current angleMode. Values are returned in the range -1 to 1.

**รูปแบบการใช้งาน**

cos ( angle )

**พารามิเตอร์**

- ``angle``  Number: มุม

.. ``angle``  Number: the angle

**ค่าที่ส่งออกมา**

- Number: โคไซน์ของมุม

.. Number: the cosine of the angle

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var a = 0.0;
	var inc = TWO_PI/25.0;
	for (var i = 0; i < 25; i++) {
	  line(i*4, 50, i*4, 50+cos(a)*40.0);
	  a = a + inc;
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
