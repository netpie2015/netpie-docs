.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

directionalLight()
==================

Creates a directional light with a color and a direction

**รูปแบบการใช้งาน**

directionalLight ( v1, [v2], [v3], [a], x, [y], [z] )

**พารามิเตอร์**

- ``v1``  Number,Array,String,p5.Color: gray value, red or hue value (depending on the current color mode), or color Array, or CSS color string

- ``v2``  Number: optional: green or saturation value

- ``v3``  Number: optional: blue or brightness value

- ``a``  Number: optional: opacity

- ``x``  Number,p5.Vector: x axis direction or a p5.Vector

- ``y``  Number: optional: y axis direction

- ``z``  Number: optional: z axis direction


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup(){
	  createCanvas(100, 100, WEBGL);
	}
	function draw(){
	  background(0);
	  //move your mouse to change light direction
	  var dirX = (mouseX / width - 0.5) *2;
	  var dirY = (mouseY / height - 0.5) *(-2);
	  directionalLight(250, 250, 250, dirX, dirY, 0.25);
	  ambientMaterial(250);
	  sphere(50);
	}


	</script>

	<br><br>

.. toctree::

