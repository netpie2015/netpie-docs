.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

set()
=====

ตั้งค่าคอมโพเนนต์ x, y และ z ของเวกเตอร์โดยใช้ตัวแปรแยกสองหรือสามตัวแปรข้อมูลจาก p5.Matrix หรือค่าจากอาร์เรย์ float

.. Sets the x, y, and z component of the vector using two or three separate
.. variables, the data from a p5.Matrix, or the values from a float array.

**รูปแบบการใช้งาน**

set ( [inMatrix], [n00..n33] )

**พารามิเตอร์**

- ``inMatrix``  p5.Matrix,Float32Array,Array: input p5.Matrix หรือ Array มีความยาว 16

- ``n00..n33``  Number: 16 หมายเลขที่ส่งผ่านค่าเพื่อหลีกเลี่ยงการคัดลอกอาร์เรย์

.. ``inMatrix``  p5.Matrix,Float32Array,Array: the input p5.Matrix or an Array of length 16
.. ``n00..n33``  Number: 16 numbers passed by value to avoid array copying.

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
