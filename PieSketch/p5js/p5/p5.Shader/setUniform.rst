.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

setUniform()
============

ห่อหุ้มรอบฟังก์ชัน gl.uniform เนื่องจากเราจัดเก็บข้อมูลชุดข้อมูลไว้ใน shader เราสามารถใช้เพื่อตรวจสอบชนิดข้อมูลที่ให้มาและเรียกใช้ฟังก์ชันที่เหมาะสม

.. Wrapper around gl.uniform functions.
.. As we store uniform info in the shader we can use that
.. to do type checking on the supplied data and call
.. the appropriate function.
**รูปแบบการใช้งาน**

setUniform ( [String], ] )

**พารามิเตอร์**

- ``String``  uniformName: ชื่อของเครื่องแบบในโปรแกรม shader

- ``]``  data: ข้อมูลที่จะเชื่อมโยงกับเครื่องแบบนั้น ประเภทอาจแตกต่างกัน (อาจเป็นค่าตัวเลขเดียว array, matrix หรือ texture / sampler reference)

.. ``String``  uniformName: the name of the uniform in the
shader program
.. ``]``  data: the data to be associated with that uniform; type
varies (could be a single numerical value, array, matrix, or
texture / sampler reference)

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
