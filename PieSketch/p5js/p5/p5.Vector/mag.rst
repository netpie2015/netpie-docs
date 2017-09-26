.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

mag()
=====

คำนวณขนาด (ความยาว) ของเวกเตอร์และส่งกลับผลลัพธ์เป็น float (นี่เป็นเพียงสมการ sqrt (x * x + y * y + z * z))

.. Calculates the magnitude (length) of the vector and returns the result as
.. a float (this is simply the equation sqrt(x*x + y*y + z*z).)

**รูปแบบการใช้งาน**

mag ( )

**ค่าที่ส่งออกมา**

- Number: ขนาดของเวกเตอร์

.. Number: magnitude of the vector

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var v = createVector(20.0, 30.0, 40.0);
	var m = v.mag();
	print(m); // Prints "53.85164807134504"

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
