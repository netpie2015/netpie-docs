.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

getAttributeCount()
===================

นับจำนวนแอตทริบิวต์ขององค์ประกอบที่ระบุซึ่งส่งกลับเป็นตัวเลข

.. Counts the specified element's number of attributes, returned as an Number.
**รูปแบบการใช้งาน**

getAttributeCount ( )

**ค่าที่ส่งออกมา**

- Number: 

.. Number: 

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
	  print(firstChild.getAttributeCount());
	}
	
	// Sketch prints:
	// 2

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
