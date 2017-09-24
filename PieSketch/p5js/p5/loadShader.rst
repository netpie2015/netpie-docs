.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

loadShader()
============

Loads a custom shader from the provided vertex and fragment
shader paths. The shader files are loaded asynchronously in the
background, so this method should be used in preload().
For now, there are three main types of shaders. p5 will automatically
supply appropriate vertices, normals, colors, and lighting attributes
if the parameters defined in the shader match the names.

**รูปแบบการใช้งาน**

loadShader ( [vertFilename], [fragFilename] )

**พารามิเตอร์**

- ``vertFilename``  String: path to file containing vertex shader source code

- ``fragFilename``  String: path to file containing fragment shader source code


**ค่าที่ส่งออกมา**

- p5.Shader: a shader object created from the provided vertex and fragment shader files.


.. toctree::

