.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

getURL()
========

Gets the current URL.

**รูปแบบการใช้งาน**

getURL ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var url;
	var x = 100;
	
	function setup() {
	  fill(0);
	  noStroke();
	  url = getURL();
	}
	
	function draw() {
	  background(200);
	  text(url, x, height/2);
	  x--;
	}
	</script>

	<br><br>

.. toctree::

