.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

alpha()
=======

อ่านค่าความเข้มจากสีหรือ pixel

**รูปแบบการใช้งาน**

alpha (*color*)

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	    noStroke();
	    c = color(0, 126, 255, 102);
	    fill(c);
	    rect(15, 15, 35, 70);
	    value = alpha(c);  // Sets 'value' to 102
	    fill(value);
	    rect(50, 15, 35, 70);
	}
	</script>


.. toctree::
	:maxdepth: 2
