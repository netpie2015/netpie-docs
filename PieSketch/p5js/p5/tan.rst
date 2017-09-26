.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

tan()
=====

คำนวณสัมผัสของมุม ฟังก์ชันนี้คำนึงถึงมุมมองปัจจุบัน ค่าจะถูกส่งกลับในช่วง -1 ถึง 1

.. Calculates the tangent of an angle. This function takes into account
.. the current angleMode. Values are returned in the range -1 to 1.

**รูปแบบการใช้งาน**

tan ( angle )

**พารามิเตอร์**

- ``angle``  Number: มุม

.. ``angle``  Number: the angle

**ค่าที่ส่งออกมา**

- Number: การสัมผัสกันของมุม

.. Number: the tangent of the angle

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	  var a = 0.0;
	  var inc = TWO_PI/50.0;
	  for (var i = 0; i < 100; i = i+2) {
	    line(i, 50, i, 50+tan(a)*2.0);
	    a = a + inc;
	  }

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
