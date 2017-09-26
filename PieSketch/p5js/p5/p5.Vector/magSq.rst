.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

magSq()
=======

คำนวณสมการกำลังสองของเวกเตอร์และส่งกลับผลลัพธ์เป็นลอย (นี่เป็นเพียงสมการ (x * x + y * y + z * z) ) เร็วขึ้นถ้าความยาวจริงไม่จำเป็นต้องใช้ในกรณีเปรียบเทียบเวกเตอร์ เป็นต้น

.. Calculates the squared magnitude of the vector and returns the result
.. as a float (this is simply the equation (x*x + y*y + z*z).)
.. Faster if the real length is not required in the
.. case of comparing vectors, etc.
**รูปแบบการใช้งาน**

magSq ( )

**ค่าที่ส่งออกมา**

- number: squared ขนาดของเวกเตอร์

.. number: squared magnitude of the vector

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Static method
	var v1 = createVector(6, 4, 2);
	print(v1.magSq()); // Prints "56"

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
