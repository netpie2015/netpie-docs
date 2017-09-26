.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

shader()
========

ฟังก์ชัน shader () ช่วยให้ผู้ใช้มี shader ที่กำหนดเองเพื่อเติมรูปร่างในโหมด WEBGL ผู้ใช้สามารถสร้าง shaders ของตนเองโดยการโหลด vertex และ shaders ส่วนด้วย loadShader ()

.. The shader() function lets the user provide a custom shader
.. to fill in shapes in WEBGL mode. Users can create their
.. own shaders by loading vertex and fragment shaders with
.. loadShader().

**รูปแบบการใช้งาน**

shader ( [s] )

**พารามิเตอร์**

- ``s``  p5.Shader: p5.Shader ที่ต้องการเพื่อใช้สำหรับการแสดงผลรูปร่าง

.. ``s``  p5.Shader: the desired p5.Shader to use for rendering shapes.

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
