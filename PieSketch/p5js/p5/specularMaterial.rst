.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

specularMaterial()
==================

Specular material for geometry with a given color. You can view all
possible materials in this
example.

**รูปแบบการใช้งาน**

specularMaterial ( v1, [v2], [v3], [a] )

**พารามิเตอร์**

- ``v1``  Number,Array,String,p5.Color: gray value, red or hue value (depending on the current color mode), or color Array, or CSS color string

- ``v2``  Number: optional: green or saturation value

- ``v3``  Number: optional: blue or brightness value

- ``a``  Number: optional: opacity


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup(){
	  createCanvas(100, 100, WEBGL);
	}
	function draw(){
	 background(0);
	 ambientLight(100);
	 pointLight(250, 250, 250, 100, 100, 0);
	 specularMaterial(250);
	 sphere(50);
	}

	</script>

	<br><br>

.. toctree::

