.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

noise()
=======

Returns the Perlin noise value at specified coordinates. Perlin noise is
a random sequence generator producing a more natural ordered, harmonic
succession of numbers compared to the standard random() function.
It was invented by Ken Perlin in the 1980s and been used since in
graphical applications to produce procedural textures, natural motion,
shapes, terrains etc. The main difference to the
random() function is that Perlin noise is defined in an infinite
n-dimensional space where each pair of coordinates corresponds to a
fixed semi-random value (fixed only for the lifespan of the program; see
the noiseSeed() function). p5.js can compute 1D, 2D and 3D noise,
depending on the number of coordinates given. The resulting value will
always be between 0.0 and 1.0. The noise value can be animated by moving
through the noise space as demonstrated in the example above. The 2nd
and 3rd dimension can also be interpreted as time.The actual
noise is structured similar to an audio signal, in respect to the
function's use of frequencies. Similar to the concept of harmonics in
physics, perlin noise is computed over several octaves which are added
together for the final result. Another way to adjust the
character of the resulting sequence is the scale of the input
coordinates. As the function works within an infinite space the value of
the coordinates doesn't matter as such, only the distance between
successive coordinates does (eg. when using noise() within a
loop). As a general rule the smaller the difference between coordinates,
the smoother the resulting noise sequence will be. Steps of 0.005-0.03
work best for most applications, but this will differ depending on use.

**รูปแบบการใช้งาน**

noise ( x, [y], [z] )

**พารามิเตอร์**

- ``x``  Number: x-coordinate in noise space

- ``y``  Number: y-coordinate in noise space

- ``z``  Number: z-coordinate in noise space


**ค่าที่ส่งออกมา**

- Number: Perlin noise value (between 0 and 1) at specified coordinates


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var xoff = 0.0;
	
	function draw() {
	  background(204);
	  xoff = xoff + .01;
	  var n = noise(xoff) * width;
	  line(n, 0, n, height);
	}


	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var noiseScale=0.02;
	
	function draw() {
	  background(0);
	  for (var x=0; x < width; x++) {
	    var noiseVal = noise((mouseX+x)*noiseScale, mouseY*noiseScale);
	    stroke(noiseVal*255);
	    line(x, mouseY+noiseVal*80, x, height);
	  }
	}


	</script>

	<br><br>

.. toctree::

