.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

set()
=====

Changes the value of key if in it already exists in
in the Dictionary otherwise makes a new key-value pair

**รูปแบบการใช้งาน**

set ( key, value )

**พารามิเตอร์**

- ``key``  Number,String: 

- ``value``  Number,String: 


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	function setup() {
	  var myDictionary = createStringDict('p5', 'js');
	  myDictionary.set('p5', 'JS');
	  myDictionary.print()
	  // above logs "key: p5 - value: JS" to console
	}
	

	</script>

	<br><br>

.. toctree::

