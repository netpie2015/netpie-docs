.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

attribute()
===========

เพิ่มแอ็ตทริบิวต์ใหม่หรือเปลี่ยนแปลงค่าของแอ็ตทริบิวต์ที่มีอยู่ในอิลิเมนต์ที่ระบุ ถ้าไม่มีค่าระบุส่งกลับค่าของแอ็ตทริบิวต์ที่กำหนดหรือเป็นค่าว่างหากไม่มีการตั้งค่าแอตทริบิวต์

.. Adds a new attribute or changes the value of an existing attribute
.. on the specified element. If no value is specified, returns the
.. value of the given attribute, or null if attribute is not set.

**รูปแบบการใช้งาน**

attribute ( attr, [value] )

**พารามิเตอร์**

- ``attr``  String: แอตทริบิวต์ที่จะตั้งค่า

- ``value``  String: ค่าที่กำหนดให้กับแอตทริบิวต์

.. ``attr``  String: attribute to set
.. ``value``  String: value to assign to attribute

**ค่าที่ส่งออกมา**

- String,Object,p5.Element: ค่าของแอตทริบิวต์ถ้าไม่มีระบุค่าหรือ p5.Element

.. String,Object,p5.Element: value of attribute, if no value is specified or p5.Element

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var myDiv = createDiv("I like pandas.");
	myDiv.attribute("align", "center");

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
