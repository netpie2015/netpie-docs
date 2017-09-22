.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

blue()
======

อ่านค่าความเข้มสีน้ำเงินจากสีหรือ pixel

**รูปแบบการใช้งาน**

blue (*color*)

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	    c = color(175, 100, 220);  // Define color 'c'
	    fill(c);  // Use color variable 'c' as fill color
	    rect(15, 20, 35, 60);  // Draw left rectangle

	    blueValue = blue(c);  // Get blue in 'c'
	    print(blueValue);  // Prints "220.0"
	    fill(0, 0, blueValue);  // Use 'blueValue' in new fill
	    rect(50, 20, 35, 60);  // Draw right rectangle
	}
	</script>


.. toctree::
	:maxdepth: 2
