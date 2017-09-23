.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

keyIsDown()
===========

The keyIsDown() function checks if the key is currently down, i.e. pressed.
It can be used if you have an object that moves, and you want several keys
to be able to affect its behaviour simultaneously, such as moving a
sprite diagonally. You can put in any number representing the keyCode of
the key, or use any of the variable keyCode names listed
<a href="http://p5js.org/reference/#p5/keyCode">here</a>.

**รูปแบบการใช้งาน**

keyIsDown ( code )

**พารามิเตอร์**

- ``code``  : The key to check for.


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var x = 100;
	var y = 100;
	
	function setup() {
	  createCanvas(512, 512);
	}
	
	function draw() {
	  if (keyIsDown(LEFT_ARROW))
	    x-=5;
	
	  if (keyIsDown(RIGHT_ARROW))
	    x+=5;
	
	  if (keyIsDown(UP_ARROW))
	    y-=5;
	
	  if (keyIsDown(DOWN_ARROW))
	    y+=5;
	
	  clear();
	  fill(255, 0, 0);
	  ellipse(x, y, 50, 50);
	}
	</script>

	<br><br>

.. toctree::

