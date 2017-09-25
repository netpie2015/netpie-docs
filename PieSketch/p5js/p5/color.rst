.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

color()
=======

Creates colors for storing in variables of the color datatype. The
parameters are interpreted as RGB or HSB values depending on the
current colorMode(). The default mode is RGB values from 0 to 255
and, therefore, the function call color(255, 204, 0) will return a
bright yellow color.

Note that if only one value is provided to color(), it will be interpreted
as a grayscale value. Add a second value, and it will be used for alpha
transparency. When three values are specified, they are interpreted as
either RGB or HSB values. Adding a fourth value applies alpha
transparency.

If a single string argument is provided, RGB, RGBA and Hex CSS color
strings and all named color strings are supported. In this case, an alpha
number value as a second argument is not supported, the RGBA form should be
used.

**รูปแบบการใช้งาน**

color ( gray, [alpha] )

**พารามิเตอร์**

- ``gray``  Number: number specifying value between white and black.

- ``alpha``  Number: alpha value relative to current color range (default is 0-255)


**ค่าที่ส่งออกมา**

- p5.Color: resulting color


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var c = color(255, 204, 0);  // Define color 'c'
	fill(c);  // Use color variable 'c' as fill color
	noStroke();  // Don't draw a stroke around shapes
	rect(30, 20, 55, 55);  // Draw rectangle

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	var c = color(255, 204, 0);  // Define color 'c'
	fill(c);  // Use color variable 'c' as fill color
	noStroke();  // Don't draw a stroke around shapes
	ellipse(25, 25, 80, 80);  // Draw left circle
	
	// Using only one value with color()
	// generates a grayscale value.
	var c = color(65);  // Update 'c' with grayscale value
	fill(c);  // Use updated 'c' as fill color
	ellipse(75, 75, 80, 80);  // Draw right circle

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	// Named SVG & CSS colors may be used,
	var c = color('magenta');
	fill(c);  // Use 'c' as fill color
	noStroke();  // Don't draw a stroke around shapes
	rect(20, 20, 60, 60);  // Draw rectangle

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	// as can hex color codes:
	noStroke();  // Don't draw a stroke around shapes
	var c = color('#0f0');
	fill(c);  // Use 'c' as fill color
	rect(0, 10, 45, 80);  // Draw rectangle
	
	c = color('#00ff00');
	fill(c);  // Use updated 'c' as fill color
	rect(55, 10, 45, 80);  // Draw rectangle

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	// RGB and RGBA color strings are also supported:
	// these all set to the same color (solid blue)
	var c;
	noStroke();  // Don't draw a stroke around shapes
	c = color('rgb(0,0,255)');
	fill(c); // Use 'c' as fill color
	rect(10, 10, 35, 35);  // Draw rectangle
	
	c = color('rgb(0%, 0%, 100%)');
	fill(c); // Use updated 'c' as fill color
	rect(55, 10, 35, 35);  // Draw rectangle
	
	c = color('rgba(0, 0, 255, 1)');
	fill(c); // Use updated 'c' as fill color
	rect(10, 55, 35, 35);  // Draw rectangle
	
	c = color('rgba(0%, 0%, 100%, 1)');
	fill(c); // Use updated 'c' as fill color
	rect(55, 55, 35, 35);  // Draw rectangle

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	// HSL color is also supported and can be specified
	// by value
	var c;
	noStroke();  // Don't draw a stroke around shapes
	c = color('hsl(160, 100%, 50%)');
	fill(c);  // Use 'c' as fill color
	rect(0, 10, 45, 80);  // Draw rectangle
	
	c = color('hsla(160, 100%, 50%, 0.5)');
	fill(c); // Use updated 'c' as fill color
	rect(55, 10, 45, 80);  // Draw rectangle

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	// HSB color is also supported and can be specified
	// by value
	var c;
	noStroke();  // Don't draw a stroke around shapes
	c = color('hsb(160, 100%, 50%)');
	fill(c);  // Use 'c' as fill color
	rect(0, 10, 45, 80);  // Draw rectangle
	
	c = color('hsba(160, 100%, 50%, 0.5)');
	fill(c); // Use updated 'c' as fill color
	rect(55, 10, 45, 80);  // Draw rectangle

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	var c;  // Declare color 'c'
	noStroke();  // Don't draw a stroke around shapes
	
	// If no colorMode is specified, then the
	// default of RGB with scale of 0-255 is used.
	c = color(50, 55, 100);  // Create a color for 'c'
	fill(c);  // Use color variable 'c' as fill color
	rect(0, 10, 45, 80);  // Draw left rect
	
	colorMode(HSB, 100);  // Use HSB with scale of 0-100
	c = color(50, 55, 100);  // Update 'c' with new color
	fill(c);  // Use updated 'c' as fill color
	rect(55, 10, 45, 80);  // Draw right rect

	</script>

	<br><br>

.. toctree::

