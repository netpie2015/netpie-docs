.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

add()
=====

เพิ่มองค์ประกอบ x, y และ z ลงในเวกเตอร์เพิ่มเวกเตอร์หนึ่งไปอีกอันหนึ่งหรือเพิ่มเวกเตอร์อิสระสองตัวเข้าด้วยกัน รุ่นของวิธีการที่เพิ่มสองเวกเตอร์ร่วมกันเป็นวิธีการแบบคงที่และส่งกลับค่า p5.Vector อื่น ๆ จะทำหน้าที่โดยตรงบนเวกเตอร์ ดูตัวอย่างสำหรับบริบทเพิ่มเติม

.. Adds x, y, and z components to a vector, adds one vector to another, or
.. adds two independent vectors together. The version of the method that adds
.. two vectors together is a static method and returns a p5.Vector, the others
.. acts directly on the vector. See the examples for more context.
**รูปแบบการใช้งาน**

add ( x, [y], [z] )

**พารามิเตอร์**

- ``x``  Number,p5.Vector,Array: คอมโพเนนต์ x ของเวกเตอร์ที่จะเพิ่มหรือ p5.Vector หรือ Array

- ``y``  Number: องค์ประกอบ y ของเวกเตอร์ที่จะเพิ่ม

- ``z``  Number: องค์ประกอบ z ของเวกเตอร์ที่จะเพิ่ม

.. ``x``  Number,p5.Vector,Array: the x component of the vector to be
                                     added or a p5.Vector or an Array
.. ``y``  Number: the y component of the vector to be
                                     added
.. ``z``  Number: the z component of the vector to be
                                     added

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var v = createVector(1, 2, 3);
	v.add(4,5,6);
	// v's components are set to [5, 7, 9]

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Static method
	var v1 = createVector(1, 2, 3);
	var v2 = createVector(2, 3, 4);
	
	var v3 = p5.Vector.add(v1, v2);
	// v3 has components [3, 5, 7]

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
