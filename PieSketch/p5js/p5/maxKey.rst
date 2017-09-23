.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

maxKey()
========

Return the highest key.

**รูปแบบการใช้งาน**

maxKey ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var myDictionary = createNumberDict({ 2 : 4, 4 : 6, 1.2 : 3});
	  var highestKey = myDictionary.maxKey(); // value is 4
	}
	</script>

	<br><br>

.. toctree::

