.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

mouseIsPressed
================

ตัวแปรระบบบูลีน mouseIsPressed เป็นจริงหากเมาส์ถูกกดและเท็จถ้าไม่

.. The boolean system variable mouseIsPressed is true if the mouse is pressed
.. and false if not.
**รูปแบบการใช้งาน**

mouseIsPressed

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function draw() {
	  background(237, 34, 93);
	  fill(0);
	
	  if (mouseIsPressed)
	    ellipse(50, 50, 50, 50);
	  else
	    rect(25, 25, 50, 50);
	
	  print(mouseIsPressed);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
