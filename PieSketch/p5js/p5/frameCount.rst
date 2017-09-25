.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

frameCount
============

The system variable frameCount contains the number of frames that have
been displayed since the program started. Inside setup() the value is 0,
after the first iteration of draw it is 1, etc.

**รูปแบบการใช้งาน**

frameCount

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	    function setup() {
	      frameRate(30);
	      textSize(20);
	      textSize(30);
	      textAlign(CENTER);
	    }
	
	    function draw() {
	      background(200);
	      text(frameCount, width/2, height/2);
	    }
	  

	</script>

	<br><br>

.. toctree::

