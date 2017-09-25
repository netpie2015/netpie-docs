.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

size()
======

Sets the width and height of the element. AUTO can be used to
only adjust one dimension. If no arguments given returns the width and height
of the element in an object.

**รูปแบบการใช้งาน**

size ( [w], [h] )

**พารามิเตอร์**

- ``w``  Number: width of the element

- ``h``  Number: height of the element


**ค่าที่ส่งออกมา**

- Object,p5.Element: 


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var div = createDiv('this is a div');
	div.size(100, 100);

	</script>

	<br><br>

.. toctree::

