.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

createElement()
===============

Creates element with given tag in the DOM with given content.
Appends to the container node if one is specified, otherwise
appends to body.

**รูปแบบการใช้งาน**

createElement ( tag, [content] )

**พารามิเตอร์**

- ``tag``  String: tag for the new element

- ``content``  String: html content to be inserted into the element


**ค่าที่ส่งออกมา**

- Object,p5.Element: pointer to p5.Element holding created node


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var h2 = createElement('h2','im an h2 p5.element!');

	</script>

	<br><br>

.. toctree::

