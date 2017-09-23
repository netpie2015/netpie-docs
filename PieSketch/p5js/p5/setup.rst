.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

setup()
=======

The setup() function is called once when the program starts. It's used to
define initial environment properties such as screen size and background
color and to load media such as images and fonts as the program starts.
There can only be one setup() function for each program and it shouldn't
be called again after its initial execution.

Note: Variables declared within setup() are not accessible within other
functions, including draw().

**รูปแบบการใช้งาน**

setup ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var a = 0;
	
	function setup() {
	  background(0);
	  noStroke();
	  fill(102);
	}
	
	function draw() {
	  rect(a++%width, 10, 2, 80);
	}
	</script>

	<br><br>

.. toctree::

