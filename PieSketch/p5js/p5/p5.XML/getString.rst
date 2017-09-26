.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

getString()
===========

ส่งคืนค่าแอตทริบิวต์ของอิลิเมนต์เป็น String ถ้ามีระบุพารามิเตอร์ defaultValue และไม่มีแอตทริบิวต์แล้วค่า defaultValue จะถูกส่งคืน ถ้าไม่มีการระบุ defaultValue และไม่มีแอตทริบิวต์ค่า null จะถูกส่งกลับ

.. Returns an attribute value of the element as an String. If the defaultValue
.. parameter is specified and the attribute doesn't exist, then defaultValue
.. is returned. If no defaultValue is specified and the attribute doesn't
.. exist, null is returned.
**รูปแบบการใช้งาน**

getString ( name, [defaultValue] )

**พารามิเตอร์**

- ``name``  String: ไม่ใช่ชื่อเต็มของแอตทริบิวต์

- ``defaultValue``  Number: ค่าเริ่มต้นของแอตทริบิวต์

.. ``name``  String: the non-null full name of the attribute
.. ``defaultValue``  Number: the default value of the attribute

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
	  print(firstChild.getString("species"));
	}
	
	// Sketch prints:
	// "Capra hircus"

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
