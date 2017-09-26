.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

loadShader()
============

โหลด shader แบบกำหนดเองจากจุดสุดยอดและเส้นทาง shader ส่วนหัว ไฟล์ shader ถูกโหลดแบบอะซิงโครนัสในพื้นหลังดังนั้นวิธีนี้ควรใช้ใน preload () ตอนนี้มีสามประเภทหลักของ shaders p5 จะจัดหาจุดสีปกติและสีที่เหมาะสมโดยอัตโนมัติหากพารามิเตอร์ที่กำหนดไว้ใน shader ตรงกับชื่อ

.. Loads a custom shader from the provided vertex and fragment
.. shader paths. The shader files are loaded asynchronously in the
.. background, so this method should be used in preload().
.. For now, there are three main types of shaders. p5 will automatically
.. supply appropriate vertices, normals, colors, and lighting attributes
.. if the parameters defined in the shader match the names.

**รูปแบบการใช้งาน**

loadShader ( [vertFilename], [fragFilename] )

**พารามิเตอร์**

- ``vertFilename``  String: เส้นทางไปยังแฟ้มที่มีรหัสแหล่งที่มาของ shader vertex

- ``fragFilename``  String: เส้นทางไปยังแฟ้มที่มีรหัสแหล่งที่มา shader ส่วน

.. ``vertFilename``  String: path to file containing vertex shader source code
.. ``fragFilename``  String: path to file containing fragment shader source code

**ค่าที่ส่งออกมา**

- p5.Shader: วัตถุ shader ที่สร้างขึ้นจากไฟล์ vertex และ shader fragment

.. p5.Shader: a shader object created from the provided vertex and fragment shader files.

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
