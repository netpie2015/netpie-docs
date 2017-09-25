.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

removeChild()
=============

Removes the element specified by name or index.

**รูปแบบการใช้งาน**

removeChild ( name )

**พารามิเตอร์**

- ``name``  String,Number: element name or index


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
	  xml.removeChild("animal");
	  var children = xml.getChildren();
	  for (var i=0; i<children.length; i++) {
	    print(children[i].getContent());
	  }
	}
	
	// Sketch prints:
	// "Leopard"
	// "Zebra"
	var xml;
	
	function preload() {
	  xml = loadXML("assets/mammals.xml");
	}
	
	function setup() {
	  xml.removeChild(1);
	  var children = xml.getChildren();
	  for (var i=0; i<children.length; i++) {
	    print(children[i].getContent());
	  }
	}
	
	// Sketch prints:
	// "Goat"
	// "Zebra"

	</script>

	<br><br>

.. toctree::

