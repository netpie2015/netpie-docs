.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

hasAttribute()
==============

ตรวจสอบว่าองค์ประกอบมีแอตทริบิวต์ที่ระบุหรือไม่

.. Checks whether or not an element has the specified attribute.

**รูปแบบการใช้งาน**

hasAttribute ( the )

**พารามิเตอร์**

- ``the``  String: แอตทริบิวต์ที่จะตรวจสอบ

.. ``the``  String: attribute to be checked

**ค่าที่ส่งออกมา**

- boolean: true ถ้าแอตทริบิวต์พบ false อื่น

.. boolean: true if attribute found else false

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
	  print(firstChild.hasAttribute("species"));
	  print(firstChild.hasAttribute("color"));
	}
	
	// Sketch prints:
	// true
	// false

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
