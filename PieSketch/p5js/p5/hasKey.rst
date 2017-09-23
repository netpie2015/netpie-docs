.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

hasKey()
========

Returns true if key exists in Dictionary
otherwise returns false

**รูปแบบการใช้งาน**

hasKey ( key )

**พารามิเตอร์**

- ``key``  : that you want to access


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	function setup() {
	  var myDictionary = createStringDict('p5', 'js');
	  print(myDictionary.hasKey('p5')); // logs true to console
	}
	
	</script>

	<br><br>

.. toctree::

