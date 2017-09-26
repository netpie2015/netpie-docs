.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

set()
=====

ตั้งค่าคอมโพเนนต์ x, y และ z ของเวกเตอร์โดยใช้ตัวแปรแยกสองหรือสามตัวแปรข้อมูลจาก p5.Vector หรือค่าจากอาร์เรย์ float

.. Sets the x, y, and z component of the vector using two or three separate
.. variables, the data from a p5.Vector, or the values from a float array.
**รูปแบบการใช้งาน**

set ( [x], [y], [z] )

**พารามิเตอร์**

- ``x``  Number,p5.Vector,Array: คอมโพเนนต์ x ของเวกเตอร์หรือ p5.Vector หรือ Array

- ``y``  Number: องค์ประกอบ y ของเวกเตอร์

- ``z``  Number: องค์ประกอบ z ของเวกเตอร์

.. ``x``  Number,p5.Vector,Array: the x component of the vector or a
                                    p5.Vector or an Array
.. ``y``  Number: the y component of the vector
.. ``z``  Number: the z component of the vector

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	   var v = createVector(1, 2, 3);
	   v.set(4,5,6); // Sets vector to [4, 5, 6]
	
	   var v1 = createVector(0, 0, 0);
	   var arr = [1, 2, 3];
	   v1.set(arr); // Sets vector to [1, 2, 3]
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
