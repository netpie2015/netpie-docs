.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

getNum()
========

Returns an attribute value of the element as an Number. If the defaultValue
parameter is specified and the attribute doesn't exist, then defaultValue
is returned. If no defaultValue is specified and the attribute doesn't
exist, the value 0 is returned.

**รูปแบบการใช้งาน**

getNum ( name, [defaultValue] )

**พารามิเตอร์**

- ``name``  String: the non-null full name of the attribute

- ``defaultValue``  Number: the default value of the attribute


**ค่าที่ส่งออกมา**

- Number: 


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
	  print(firstChild.getNum("id"));
	}
	
	// Sketch prints:
	// 0

	</script>

	<br><br>

.. toctree::

