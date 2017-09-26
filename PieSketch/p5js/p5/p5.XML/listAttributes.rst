.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

listAttributes()
================

รับแอตทริบิวต์ขององค์ประกอบที่ระบุทั้งหมดและส่งค่าเป็นอาร์เรย์ของสตริง

.. Gets all of the specified element's attributes, and returns them as an
.. array of Strings.
**รูปแบบการใช้งาน**

listAttributes ( )

**ค่าที่ส่งออกมา**

- Array.<String>: สตริงของสตริงที่มีชื่อของแอตทริบิวต์

.. Array.<String>: an array of strings containing the names of attributes

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
	  print(firstChild.listAttributes());
	}
	
	// Sketch prints:
	// ["id", "species"]

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
