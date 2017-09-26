.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

sub()
=====

ลบเซต x, y และ z จากเวกเตอร์ลบเวกเตอร์หนึ่งจากอีกอันหนึ่งหรือลบสองเวกเตอร์อิสระ รุ่นของวิธีการที่ลบสองเวกเตอร์เป็นวิธีการแบบคงที่และส่งกลับค่า p5.Vector การกระทำอื่น ๆ โดยตรงบนเวกเตอร์ ดูตัวอย่างสำหรับบริบทเพิ่มเติม

.. Subtracts x, y, and z components from a vector, subtracts one vector from
.. another, or subtracts two independent vectors. The version of the method
.. that subtracts two vectors is a static method and returns a p5.Vector, the
.. other acts directly on the vector. See the examples for more context.

**รูปแบบการใช้งาน**

sub ( x, [y], [z] )

**พารามิเตอร์**

- ``x``  Number,p5.Vector,Array: คอมโพเนนต์ x ของเวกเตอร์หรือ p5.Vector หรือ Array

- ``y``  Number: องค์ประกอบ y ของเวกเตอร์

- ``z``  Number: องค์ประกอบ z ของเวกเตอร์

.. ``x``  Number,p5.Vector,Array: the x component of the vector or a p5.Vector or an Array
.. ``y``  Number: the y component of the vector
.. ``z``  Number: the z component of the vector

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var v = createVector(4, 5, 6);
	v.sub(1, 1, 1);
	// v's components are set to [3, 4, 5]

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	// Static method
	var v1 = createVector(2, 3, 4);
	var v2 = createVector(1, 2, 3);
	
	var v3 = p5.Vector.sub(v1, v2);
	// v3 has components [1, 1, 1]

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
