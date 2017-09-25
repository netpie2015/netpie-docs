.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

attribute()
===========

Adds a new attribute or changes the value of an existing attribute
on the specified element. If no value is specified, returns the
value of the given attribute, or null if attribute is not set.

**รูปแบบการใช้งาน**

attribute ( attr, [value] )

**พารามิเตอร์**

- ``attr``  String: attribute to set

- ``value``  String: value to assign to attribute


**ค่าที่ส่งออกมา**

- String,Object,p5.Element: value of attribute, if no value is specified or p5.Element


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var myDiv = createDiv("I like pandas.");
	myDiv.attribute("align", "center");

	</script>

	<br><br>

.. toctree::

