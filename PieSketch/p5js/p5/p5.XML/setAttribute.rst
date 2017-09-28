.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

setAttribute()
==============

ตั้งค่าแอตทริบิวต์ขององค์ประกอบ พารามิเตอร์แรกระบุชื่อแอตทริบิวต์ในขณะที่สองระบุเนื้อหาใหม่

.. Sets the content of an element's attribute. The first parameter specifies
.. the attribute name, while the second specifies the new content.

**รูปแบบการใช้งาน**

setAttribute ( name, value )

**พารามิเตอร์**

- ``name``  String: ชื่อเต็มของแอตทริบิวต์

- ``value``  Number: ค่าของแอตทริบิวต์

.. ``name``  String: the full name of the attribute
.. ``value``  Number: the value of the attribute

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// The following short XML file called "mammals.xml" is parsed
	// in the code below.
	//
	// <?xml version="1.0"?>
	// &lt;mammals&gt;
	//   &lt;animal id="0" species="Capra hircus">Goat&lt;/animal&gt;
	//   &lt;animal id="1" species="Panthera pardus">Leopard&lt;/animal&gt;
	//   &lt;animal id="2" species="Equus zebra">Zebra&lt;/animal&gt;
	// &lt;/mammals&gt;
	
	var xml;
	
	function preload() {
	  xml = loadXML("assets/mammals.xml");
	}
	
	function setup() {
	  var firstChild = xml.getChild("animal");
	  print(firstChild.getString("species"));
	  firstChild.setAttribute("species", "Jamides zebra");
	  print(firstChild.getString("species"));
	}
	
	// Sketch prints:
	// "Capra hircus"
	// "Jamides zebra"

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
