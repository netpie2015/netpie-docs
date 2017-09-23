.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

size()
======

Returns the number of key-value pairs currently in Dictionary object

**รูปแบบการใช้งาน**

size ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	function setup() {
	  var myDictionary = createNumberDict(1, 10);
	  myDictionary.create(2, 20);
	  myDictionary.create(3, 30);
	  var amt = myDictionary.size(); // value of amt is 3
	}
	
	</script>

	<br><br>

.. toctree::

