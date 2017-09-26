.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

acos()
======

ผกผันของ cos () จะส่งค่าโคไซน์อาร์คของค่า ฟังก์ชันนี้คาดว่าค่าในช่วง -1 ถึง 1 และค่าจะถูกส่งคืนในช่วง 0 ถึง PI (3.1415927)

.. The inverse of cos(), returns the arc cosine of a value. This function
.. expects the values in the range of -1 to 1 and values are returned in
.. the range 0 to PI (3.1415927).

**รูปแบบการใช้งาน**

acos ( value )

**พารามิเตอร์**

- ``value``  Number: ค่าที่โคไซน์อาร์จะถูกส่งคืน

.. ``value``  Number: the value whose arc cosine is to be returned

**ค่าที่ส่งออกมา**

- Number: โคไซน์โคไซน์ของค่าที่กำหนด

.. Number: the arc cosine of the given value

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var a = PI;
	var c = cos(a);
	var ac = acos(c);
	// Prints: "3.1415927 : -1.0 : 3.1415927"
	print(a + " : " + c + " : " +  ac);

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	var a = PI + PI/4.0;
	var c = cos(a);
	var ac = acos(c);
	// Prints: "3.926991 : -0.70710665 : 2.3561943"
	print(a + " : " + c + " : " +  ac);

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
