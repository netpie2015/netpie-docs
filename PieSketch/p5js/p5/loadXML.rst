.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

loadXML()
=========

Reads the contents of a file and creates an XML object with its values.
If the name of the file is used as the parameter, as in the above example,
the file must be located in the sketch directory/folder.
Alternatively, the file maybe be loaded from anywhere on the local
computer using an absolute path (something that starts with / on Unix and
Linux, or a drive letter on Windows), or the filename parameter can be a
URL for a file found on a network.
This method is asynchronous, meaning it may not finish before the next
line in your sketch is executed. Calling loadXML() inside preload()
guarantees to complete the operation before setup() and draw() are called.
Outside of preload(), you may supply a callback function to handle the
object.

**รูปแบบการใช้งาน**

loadXML ( filename, [callback], [errorCallback] )

**พารามิเตอร์**

- ``filename``  String: name of the file or URL to load

- ``callback``  function: function to be executed after loadXML() completes, XML object is passed in as first argument

- ``errorCallback``  function: function to be executed if there is an error, response is passed in as first argument


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	<div class='norender'>// The following short XML file called "mammals.xml" is parsed
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
	
	  for (var i = 0; i < children.length; i++) {
	    var id = children[i].getNum("id");
	    var coloring = children[i].getString("species");
	    var name = children[i].getContent();
	    print(id + ", " + coloring + ", " + name);
	  }
	}
	
	// Sketch prints:
	// 0, Capra hircus, Goat
	// 1, Panthera pardus, Leopard
	// 2, Equus zebra, Zebra
	</script>

	<br><br>

.. toctree::

