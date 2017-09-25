.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

setUniform()
============

Wrapper around gl.uniform functions.
As we store uniform info in the shader we can use that
to do type checking on the supplied data and call
the appropriate function.

**รูปแบบการใช้งาน**

setUniform ( [String], ] )

**พารามิเตอร์**

- ``String``  uniformName: the name of the uniform in the shader program

- ``]``  data: the data to be associated with that uniform; type varies (could be a single numerical value, array, matrix, or texture / sampler reference)


.. toctree::

