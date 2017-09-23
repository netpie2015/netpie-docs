.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

minKey()
========

Return the lowest key.

**รูปแบบการใช้งาน**

minKey ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var myDictionary = createNumberDict({2 : 4, 4 : 6, 1.2 : 3});
	  var lowestKey = myDictionary.minKey(); // value is 1.2
	}
	</script>

	<br><br>

.. toctree::

