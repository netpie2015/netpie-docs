.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

texture()
=========

Texture for geometry.  You can view other possible materials in this
<a href="https://p5js.org/examples/3d-materials.html">example</a>.

**รูปแบบการใช้งาน**

texture ( tex )

**พารามิเตอร์**

- ``tex``  : 2-dimensional graphics to render as texture


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var img;
	function setup(){
	  createCanvas(100, 100, WEBGL);
	  img = loadImage("assets/laDefense.jpg");
	}
	
	function draw(){
	  background(0);
	  rotateZ(frameCount * 0.01);
	  rotateX(frameCount * 0.01);
	  rotateY(frameCount * 0.01);
	  //pass image as texture
	  texture(img);
	  box(200, 200, 200);
	}
	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	var pg;
	function setup(){
	  createCanvas(100, 100, WEBGL);
	  pg = createGraphics(200, 200);
	  pg.textSize(100);
	}
	
	function draw(){
	  background(0);
	  pg.background(255);
	  pg.text('hello!', 0, 100);
	  //pass image as texture
	  texture(pg);
	  plane(200);
	}
	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	var vid;
	function preload(){
	  vid = createVideo("assets/fingers.mov");
	  vid.hide();
	  vid.loop();
	}
	function setup(){
	  createCanvas(100, 100, WEBGL);
	}
	
	function draw(){
	  background(0);
	  //pass video frame as texture
	  texture(vid);
	  plane(200);
	}
	</script>

	<br><br>

.. toctree::

