.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

equals()
========

การตรวจสอบความเสมอภาคกับ p5.Vector

.. Equality check against a p5.Vector

**รูปแบบการใช้งาน**

equals ( [x], [y], [z] )

**พารามิเตอร์**

- ``x``  Number,p5.Vector,Array: คอมโพเนนต์ x ของเวกเตอร์หรือ p5.Vector หรือ Array

- ``y``  Number: องค์ประกอบ y ของเวกเตอร์

- ``z``  Number: องค์ประกอบ z ของเวกเตอร์

.. ``x``  Number,p5.Vector,Array: the x component of the vector or a p5.Vector or an Array
.. ``y``  Number: the y component of the vector
.. ``z``  Number: the z component of the vector

**ค่าที่ส่งออกมา**

- Boolean: ไม่ว่าจะเป็นพาหะเท่ากับ

.. Boolean: whether the vectors are equals

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	v1 = createVector(5,10,20);
	v2 = createVector(5,10,20);
	v3 = createVector(13,10,19);
	
	print(v1.equals(v2.x,v2.y,v2.z)); // true
	print(v1.equals(v3.x,v3.y,v3.z)); // false

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var v1 = createVector(10.0, 20.0, 30.0);
	var v2 = createVector(10.0, 20.0, 30.0);
	var v3 = createVector(0.0, 0.0, 0.0);
	print (v1.equals(v2)) // true
	print (v1.equals(v3)) // false

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
