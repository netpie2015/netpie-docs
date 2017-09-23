.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

minValue()
==========

Return the lowest value.

**รูปแบบการใช้งาน**

minValue ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var myDictionary = createNumberDict({2 : -10, 4 : 0.65, 1.2 : 3});
	  var lowestValue = myDictionary.minValue(); // value is -10
	}
	</script>

	<br><br>

.. toctree::

