.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

getContent()
============

ส่งกลับเนื้อหาขององค์ประกอบ หากไม่มีเนื้อหาดังกล่าวค่าดีฟอลต์จะถูกส่งกลับถ้าระบุมิฉะนั้นจะถูกส่งกลับค่า null

.. Returns the content of an element. If there is no such content,
.. defaultValue is returned if specified, otherwise null is returned.

**รูปแบบการใช้งาน**

getContent ( [defaultValue] )

**พารามิเตอร์**

- ``defaultValue``  String: ค่าที่ส่งคืนหากไม่พบเนื้อหา

.. ``defaultValue``  String: value returned if no content is found

**ค่าที่ส่งออกมา**

- String: 

.. String: 

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
	  print(firstChild.getContent());
	}
	
	// Sketch prints:
	// "Goat"

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
