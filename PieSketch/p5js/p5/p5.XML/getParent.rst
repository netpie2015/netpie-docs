.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

getParent()
===========

รับสำเนาของพาเรนต์ขององค์ประกอบ ส่งกลับผู้ปกครองเป็นอีกหนึ่งวัตถุ p5.XML

.. Gets a copy of the element's parent. Returns the parent as another
.. p5.XML object.
**รูปแบบการใช้งาน**

getParent ( )

**ค่าที่ส่งออกมา**

- p5.XML: องค์ประกอบหลัก

.. p5.XML: element parent

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
	  var children = xml.getChildren("animal");
	  var parent = children[1].getParent();
	  print(parent.getName());
	}
	
	// Sketch prints:
	// mammals

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
