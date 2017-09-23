.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

p5
==

core
----

2d_primitives
^^^^^^^^^^^^^

.. toctree::
	arc() : Draw an arc to the screen. <arc>
	ellipse() : Draws an ellipse (oval) to the screen. <ellipse>
	line() : Draws a line (a direct path between two points) to the screen. <line>
	point() : Draws a point, a coordinate in space at the dimension of one pixel. <point>
	quad() : Draw a quad. <quad>
	rect() : Draws a rectangle to the screen. <rect>
	triangle() : A triangle is a plane created by connecting three points. <triangle>

attributes
^^^^^^^^^^

.. toctree::
	textAlign() : Sets the current alignment for drawing text. <textAlign>
	textAscent() : Returns the ascent of the current font at its current size. <textAscent>
	textDescent() : Returns the descent of the current font at its current size. <textDescent>
	textLeading() : Sets/gets the spacing, in pixels, between lines of text. <textLeading>
	textSize() : Sets/gets the current font size. <textSize>
	textStyle() : Sets/gets the style of the text for system fonts to NORMAL, ITALIC, or BOLD. <textStyle>
	textWidth() : Calculates and returns the width of any character or text string. <textWidth>

core
^^^^

.. toctree::
	draw() : Called directly after setup(), the draw() function continuously executes the lines of code contained inside its block until the program is stopped or noLoop() is called. <draw>
	p5() : This is the p5 instance constructor. <p5>
	preload() : Called directly before setup(), the preload() function is used to handle asynchronous loading of external files. <preload>
	remove() : Removes the entire p5 sketch. <remove>
	setup() : The setup() function is called once when the program starts. <setup>

curves
^^^^^^

.. toctree::
	bezier() : Draws a cubic Bezier curve on the screen. <bezier>
	bezierDetail() : Sets the resolution at which Beziers display. <bezierDetail>
	bezierPoint() : Evaluates the Bezier at position t for points a, b, c, d. <bezierPoint>
	bezierTangent() : Evaluates the tangent to the Bezier at position t for points a, b, c, d. <bezierTangent>
	curve() : Draws a curved line on the screen between two points, given as the middle four parameters. <curve>
	curveDetail() : Sets the resolution at which curves display. <curveDetail>
	curvePoint() : Evaluates the curve at position t for points a, b, c, d. <curvePoint>
	curveTangent() : Evaluates the tangent to the curve at position t for points a, b, c, d. <curveTangent>
	curveTightness() : Modifies the quality of forms created with curve() and curveVertex(). <curveTightness>

environment
^^^^^^^^^^^

.. toctree::
	cursor() : Sets the cursor to a predefined symbol or an image, or makes it visible if already hidden. <cursor>
	displayDensity() : Returns the pixel density of the current display the sketch is running on. <displayDensity>
	frameRate() : Specifies the number of frames to be displayed every second. <frameRate>
	fullscreen() : If argument is given, sets the sketch to fullscreen or not based on the value of the argument. <fullscreen>
	getFrameRate() : Returns the current framerate. <getFrameRate>
	getURL() : Gets the current URL. <getURL>
	getURLParams() : Gets the current URL params as an Object. <getURLParams>
	getURLPath() : Gets the current URL path as an array. <getURLPath>
	noCursor() : Hides the cursor from view. <noCursor>
	pixelDensity() : Sets the pixel scaling for high pixel density displays. <pixelDensity>
	print() : The print() function writes to the console area of your browser. <print>
	setFrameRate() : Specifies the number of frames to be displayed every second. <setFrameRate>
	windowResized() : The windowResized() function is called once every time the browser window is resized. <windowResized>

p5.Element
^^^^^^^^^^

.. toctree::
	changed() : The .changed() function is called when the value of an element is changed. <changed>
	class() : Adds given class to the element. <class>
	doubleClicked() : The .doubleClicked() function is called once after every time a mouse button is pressed twice over the element. <doubleClicked>
	dragLeave() : The .dragLeave() function is called once after every time a dragged file leaves the element area. <dragLeave>
	dragOver() : The .dragOver() function is called once after every time a file is dragged over the element. <dragOver>
	drop() : The .drop() function is called for each file dropped on the element. <drop>
	id() : Sets the ID of the element. <id>
	input() : The .input() function is called when any user input is detected with an element. <input>
	mouseClicked() : The .mouseClicked() function is called once after a mouse button is pressed and released over the element. <mouseClicked>
	mouseMoved() : The .mouseMoved() function is called once every time a mouse moves over the element. <mouseMoved>
	mouseOut() : The .mouseOut() function is called once after every time a mouse moves off the element. <mouseOut>
	mouseOver() : The .mouseOver() function is called once after every time a mouse moves onto the element. <mouseOver>
	mousePressed() : The .mousePressed() function is called once after every time a mouse button is pressed over the element. <mousePressed>
	mouseReleased() : The .mouseReleased() function is called once after every time a mouse button is released over the element. <mouseReleased>
	mouseWheel() : The .mouseWheel() function is called once after every time a mouse wheel is scrolled over the element. <mouseWheel>
	parent() : Attaches the element to the parent specified. <parent>
	touchEnded() : The .touchEnded() function is called once after every time a touch is registered. <touchEnded>
	touchMoved() : The .touchMoved() function is called once after every time a touch move is registered. <touchMoved>
	touchStarted() : The .touchStarted() function is called once after every time a touch is registered. <touchStarted>

p5.Renderer
^^^^^^^^^^^

.. toctree::
	calculateOffset() : Helper fxn to measure ascent and descent. <calculateOffset>

rendering
^^^^^^^^^

.. toctree::
	blendMode() : Blends the pixels in the display window according to the defined mode. <blendMode>
	createCanvas() : Creates a canvas element in the document, and sets the dimensions of it in pixels. <createCanvas>
	createGraphics() : Creates and returns a new p5.Renderer object. <createGraphics>
	noCanvas() : Removes the default canvas for a p5 sketch that doesn't require a canvas <noCanvas>
	resizeCanvas() : Resizes the canvas to given width and height. <resizeCanvas>

structure
^^^^^^^^^

.. toctree::
	loop() : By default, p5.js loops through draw() continuously, executing the code within it. <loop>
	noLoop() : Stops p5.js from continuously executing the code within draw(). <noLoop>
	pop() : The push() function saves the current drawing style settings and transformations, while pop() restores these settings. <pop>
	push() : The push() function saves the current drawing style settings and transformations, while pop() restores these settings. <push>
	redraw() : Executes the code within draw() one time. <redraw>

transform
^^^^^^^^^

.. toctree::
	applyMatrix() : Multiplies the current matrix by the one specified through the parameters. <applyMatrix>
	resetMatrix() : Replaces the current matrix with the identity matrix. <resetMatrix>
	rotate() : Rotates a shape the amount specified by the angle parameter. <rotate>
	rotateX() : Rotates around X axis. <rotateX>
	rotateY() : Rotates around Y axis. <rotateY>
	rotateZ() : Rotates around Z axis. <rotateZ>
	scale() : Increases or decreases the size of a shape by expanding and contracting vertices. <scale>
	shearX() : Shears a shape around the x-axis the amount specified by the angle parameter. <shearX>
	shearY() : Shears a shape around the y-axis the amount specified by the angle parameter. <shearY>
	translate() : Specifies an amount to displace objects within the display window. <translate>

vertex
^^^^^^

.. toctree::
	beginContour() : Use the beginContour() and endContour() functions to create negative shapes within shapes such as the center of the letter 'O'. <beginContour>
	beginShape() : Using the beginShape() and endShape() functions allow creating more complex forms. <beginShape>
	bezierVertex() : Specifies vertex coordinates for Bezier curves. <bezierVertex>
	curveVertex() : Specifies vertex coordinates for curves. <curveVertex>
	endContour() : Use the beginContour() and endContour() functions to create negative shapes within shapes such as the center of the letter 'O'. <endContour>
	endShape() : The endShape() function is the companion to beginShape() and may only be called after beginShape(). <endShape>
	quadraticVertex() : Specifies vertex coordinates for quadratic Bezier curves. <quadraticVertex>
	vertex() : All shapes are constructed by connecting a series of vertices. <vertex>

color
-----

color_conversion
^^^^^^^^^^^^^^^^

.. toctree::
	ColorConversion._hsbaToHSLA() : Convert an HSBA array to HSLA. <ColorConversion._hsbaToHSLA>
	ColorConversion._hsbaToRGBA() : Convert an HSBA array to RGBA. <ColorConversion._hsbaToRGBA>
	ColorConversion._hslaToHSBA() : Convert an HSLA array to HSBA. <ColorConversion._hslaToHSBA>
	ColorConversion._hslaToRGBA() : Convert an HSLA array to RGBA. <ColorConversion._hslaToRGBA>
	ColorConversion._rgbaToHSBA() : Convert an RGBA array to HSBA. <ColorConversion._rgbaToHSBA>
	ColorConversion._rgbaToHSLA() : Convert an RGBA array to HSLA. <ColorConversion._rgbaToHSLA>

creating_reading
^^^^^^^^^^^^^^^^

.. toctree::
	alpha() : Extracts the alpha value from a color or pixel array. <alpha>
	blue() : Extracts the blue value from a color or pixel array. <blue>
	brightness() : Extracts the HSB brightness value from a color or pixel array. <brightness>
	color() : Creates colors for storing in variables of the color datatype. <color>
	green() : Extracts the green value from a color or pixel array. <green>
	hue() : Extracts the hue value from a color or pixel array. <hue>
	lerpColor() : Blends two colors to find a third color somewhere between them. <lerpColor>
	lightness() : Extracts the HSL lightness value from a color or pixel array. <lightness>
	red() : Extracts the red value from a color or pixel array. <red>
	saturation() : Extracts the saturation value from a color or pixel array. <saturation>

p5.Color
^^^^^^^^

.. toctree::
	Color._parseInputs() : For a number of different inputs, returns a color formatted as [r, g, b, a] arrays, with each component normalized between 0 and 1. <Color._parseInputs>

setting
^^^^^^^

.. toctree::
	background() : The background() function sets the color used for the background of the p5.js canvas. <background>
	clear() : Clears the pixels within a buffer. <clear>
	colorMode() : colorMode() changes the way p5.js interprets color data. <colorMode>
	fill() : Sets the color used to fill shapes. <fill>
	noFill() : Disables filling geometry. <noFill>
	noStroke() : Disables drawing the stroke (outline). <noStroke>
	stroke() : Sets the color used to draw lines and borders around shapes. <stroke>

data
----

p5.TypedDict
^^^^^^^^^^^^

.. toctree::
	add() : Add to a value stored at a certain key The sum is stored in that location in the Dictionary. <add>
	clear() : Empties Dictionary of all key-value pairs <clear>
	create() : Removes a key-value pair in the Dictionary <create>
	createNumberDict() : Creates a new instance of p5.NumberDict using the key, value pair or object you provide. <createNumberDict>
	createStringDict() : Creates a new instance of p5.StringDict using the key, value pair or object you provide. <createStringDict>
	div() : Divide a value stored at a certain key The quotient is stored in that location in the Dictionary. <div>
	get() : Returns value stored at supplied key. <get>
	hasKey() : Returns true if key exists in Dictionary otherwise returns false <hasKey>
	maxKey() : Return the highest key. <maxKey>
	maxValue() : Return the highest value. <maxValue>
	minKey() : Return the lowest key. <minKey>
	minValue() : Return the lowest value. <minValue>
	mult() : Multiply a value stored at a certain key The product is stored in that location in the Dictionary. <mult>
	print() : Logs the list of items currently in the Dictionary to the console <print>
	remove() : Removes a key-value pair in the Dictionary <remove>
	saveJSON() : Converts the Dictionary into a JSON file for local storage. <saveJSON>
	saveTable() : Converts the Dictionary into a CSV file for local storage. <saveTable>
	set() : Changes the value of key if in it already exists in in the Dictionary otherwise makes a new key-value pair <set>
	size() : Returns the number of key-value pairs currently in Dictionary object <size>
	sub() : Subtract from a value stored at a certain key The difference is stored in that location in the Dictionary. <sub>

events
------

acceleration
^^^^^^^^^^^^

.. toctree::
	deviceMoved() : The deviceMoved() function is called when the device is moved by more than the threshold value along X, Y or Z axis. <deviceMoved>
	deviceShaken() : The deviceShaken() function is called when the device total acceleration changes of accelerationX and accelerationY values is more than the threshold value. <deviceShaken>
	deviceTurned() : The deviceTurned() function is called when the device rotates by more than 90 degrees continuously. <deviceTurned>
	setMoveThreshold() : The setMoveThreshold() function is used to set the movement threshold for the deviceMoved() function. <setMoveThreshold>
	setShakeThreshold() : The setShakeThreshold() function is used to set the movement threshold for the deviceShaken() function. <setShakeThreshold>

keyboard
^^^^^^^^

.. toctree::
	areDownKeys() : The checkDownKeys function returns a boolean true if any keys pressed and a false if no keys are currently pressed. <areDownKeys>
	keyIsDown() : The keyIsDown() function checks if the key is currently down, i.e. <keyIsDown>
	keyPressed() : The keyPressed() function is called once every time a key is pressed. <keyPressed>
	keyReleased() : The keyReleased() function is called once every time a key is released. <keyReleased>
	keyTyped() : The keyTyped() function is called once every time a key is pressed, but action keys such as Ctrl, Shift, and Alt are ignored. <keyTyped>

mouse
^^^^^

.. toctree::
	doubleClicked() : The doubleClicked() function is executed every time a event listener has detected a dblclick event which is a part of the DOM L3 specification. <doubleClicked>
	mouseClicked() : The mouseClicked() function is called once after a mouse button has been pressed and then released. <mouseClicked>
	mouseDragged() : The mouseDragged() function is called once every time the mouse moves and a mouse button is pressed. <mouseDragged>
	mouseMoved() : The mouseMoved() function is called every time the mouse moves and a mouse button is not pressed. <mouseMoved>
	mousePressed() : The mousePressed() function is called once after every time a mouse button is pressed. <mousePressed>
	mouseReleased() : The mouseReleased() function is called every time a mouse button is released. <mouseReleased>
	mouseWheel() : The function mouseWheel() is executed every time a vertical mouse wheel event is detected either triggered by an actual mouse wheel or by a touchpad. <mouseWheel>

touch
^^^^^

.. toctree::
	touchEnded() : The touchEnded() function is called every time a touch ends. <touchEnded>
	touchMoved() : The touchMoved() function is called every time a touch move is registered. <touchMoved>
	touchStarted() : The touchStarted() function is called once after every time a touch is registered. <touchStarted>

image
-----

filters
^^^^^^^

.. toctree::
	apply() : Applys a filter function to a canvas. <apply>
	dilate() : reduces the bright areas in an image <dilate>
	erode() : increases the bright areas in an image <erode>
	gray() : Converts any colors in the image to grayscale equivalents. <gray>
	invert() : Sets each pixel to its inverse value. <invert>
	opaque() : Sets the alpha channel to entirely opaque. <opaque>
	posterize() : Limits each channel of the image to the number of colors specified as the parameter. <posterize>
	threshold() : Converts the image to black and white pixels depending if they are above or below the threshold defined by the level parameter. <threshold>

image
^^^^^

.. toctree::
	createImage() : Creates a new p5.Image (the datatype for storing images). <createImage>
	saveCanvas() : Save the current canvas as an image. <saveCanvas>
	saveFrames() : Capture a sequence of frames that can be used to create a movie. <saveFrames>

loading_displaying
^^^^^^^^^^^^^^^^^^

.. toctree::
	loadFont() : Loads an opentype font file (.otf, .ttf) from a file or a URL, and returns a PFont Object. <loadFont>
	text() : Draws text to the screen. <text>
	textFont() : Sets the current font that will be drawn with the text() function. <textFont>

p5.Image
^^^^^^^^

.. toctree::
	blend() : Copies a region of pixels from one image to another, using a specified blend mode to do the operation. <blend>
	copy() : Copies a region of pixels from one image to another. <copy>
	filter() : Applies an image filter to a p5.Image <filter>
	get() : Get a region of pixels from an image. <get>
	isModified() : helper method for web GL mode to figure out if the image has been modified and might need to be re-uploaded to texture memory between frames. <isModified>
	loadPixels() : Loads the pixels data for this image into the [pixels] attribute. <loadPixels>
	mask() : Masks part of an image from displaying by loading another image and using it's alpha channel as an alpha channel for this image. <mask>
	resize() : Resize the image to a new width and height. <resize>
	save() : Saves the image to a file and force the browser to download it. <save>
	set() : Set the color of a single pixel or write an image into this p5.Image. <set>
	setModified() : helper method for web GL mode to indicate that an image has been changed or unchanged since last upload. <setModified>
	updatePixels() : Updates the backing canvas for this image with the contents of the [pixels] array. <updatePixels>

pixels
^^^^^^

.. toctree::
	blend() : Copies a region of pixels from one image to another, using a specified blend mode to do the operation. <blend>
	copy() : Copies a region of the canvas to another region of the canvas and copies a region of pixels from an image used as the srcImg parameter into the canvas srcImage is specified this is used as the source. <copy>
	filter() : Applies a filter to the canvas. <filter>
	get() : Returns an array of [R,G,B,A] values for any pixel or grabs a section of an image. <get>
	loadPixels() : Loads the pixel data for the display window into the pixels[] array. <loadPixels>
	set() : Changes the color of any pixel, or writes an image directly to the display window. <set>
	updatePixels() : Updates the display window with the data in the pixels[] array. <updatePixels>

io
--

p5.Table
^^^^^^^^

.. toctree::
	addColumn() : Use addColumn() to add a new column to a Table object. <addColumn>
	addRow() : Use addRow() to add a new row of data to a p5.Table object. <addRow>
	clearRows() : Removes all rows from a Table. <clearRows>
	findRow() : Finds the first row in the Table that contains the value  provided, and returns a reference to that row. <findRow>
	findRows() : Finds the rows in the Table that contain the value  provided, and returns references to those rows. <findRows>
	get() : Retrieves a value from the Table's specified row and column. <get>
	getArray() : Retrieves all table data and returns it as a multidimensional array. <getArray>
	getColumn() : Retrieves all values in the specified column, and returns them  as an array. <getColumn>
	getNum() : Retrieves a Float value from the Table's specified row and column. <getNum>
	getObject() : Retrieves all table data and returns as an object. <getObject>
	getRow() : Returns a reference to the specified p5.TableRow. <getRow>
	getRowCount() : Returns the total number of rows in a Table. <getRowCount>
	getRows() : Gets all rows from the table. <getRows>
	getString() : Retrieves a String value from the Table's specified row and column. <getString>
	matchRow() : Finds the first row in the Table that matches the regular  expression provided, and returns a reference to that row. <matchRow>
	matchRows() : Finds the rows in the Table that match the regular expression provided,  and returns references to those rows. <matchRows>
	removeColumn() : Use removeColumn() to remove an existing column from a Table  object. <removeColumn>
	removeRow() : Removes a row from the table object. <removeRow>
	removeTokens() : Removes any of the specified characters (or "tokens"). <removeTokens>
	set() : Stores a value in the Table's specified row and column. <set>
	setNum() : Stores a Float value in the Table's specified row and column. <setNum>
	setString() : Stores a String value in the Table's specified row and column. <setString>
	trim() : Trims leading and trailing whitespace, such as spaces and tabs,  from String table values. <trim>

p5.TableRow
^^^^^^^^^^^

.. toctree::
	get() : Retrieves a value from the TableRow's specified column. <get>
	getNum() : Retrieves a Float value from the TableRow's specified  column. <getNum>
	getString() : Retrieves an String value from the TableRow's specified  column. <getString>
	set() : Stores a value in the TableRow's specified column. <set>
	setNum() : Stores a Float value in the TableRow's specified column. <setNum>
	setString() : Stores a String value in the TableRow's specified column. <setString>

p5.XML
^^^^^^

.. toctree::
	addChild() : Appends a new child to the element. <addChild>
	getAttributeCount() : Counts the specified element's number of attributes, returned as an Number. <getAttributeCount>
	getChild() : Returns the first of the element's children that matches the name parameter or the child of the given index.It returns undefined if no matching child is found. <getChild>
	getChildren() : Returns all of the element's children as an array of p5.XML objects. <getChildren>
	getContent() : Returns the content of an element. <getContent>
	getName() : Gets the element's full name, which is returned as a String. <getName>
	getNum() : Returns an attribute value of the element as an Number. <getNum>
	getParent() : Gets a copy of the element's parent. <getParent>
	getString() : Returns an attribute value of the element as an String. <getString>
	hasAttribute() : Checks whether or not an element has the specified attribute. <hasAttribute>
	hasChildren() : Checks whether or not the element has any children, and returns the result as a boolean. <hasChildren>
	listAttributes() : Gets all of the specified element's attributes, and returns them as an array of Strings. <listAttributes>
	listChildren() : Get the names of all of the element's children, and returns the names as an array of Strings. <listChildren>
	removeChild() : Removes the element specified by name or index. <removeChild>
	setAttribute() : Sets the content of an element's attribute. <setAttribute>
	setContent() : Sets the element's content. <setContent>
	setName() : Sets the element's name, which is specified as a String. <setName>

math
----

calculation
^^^^^^^^^^^

.. toctree::
	abs() : Calculates the absolute value (magnitude) of a number. <abs>
	ceil() : Calculates the closest int value that is greater than or equal to the value of the parameter. <ceil>
	constrain() : Constrains a value between a minimum and maximum value. <constrain>
	dist() : Calculates the distance between two points. <dist>
	exp() : Returns Euler's number e (2.71828...) raised to the power of the n parameter. <exp>
	floor() : Calculates the closest int value that is less than or equal to the value of the parameter. <floor>
	lerp() : Calculates a number between two numbers at a specific increment. <lerp>
	log() : Calculates the natural logarithm (the base-e logarithm) of a number. <log>
	mag() : Calculates the magnitude (or length) of a vector. <mag>
	map() : Re-maps a number from one range to another. <map>
	max() : Determines the largest value in a sequence of numbers, and then returns that value. <max>
	min() : Determines the smallest value in a sequence of numbers, and then returns that value. <min>
	norm() : Normalizes a number from another range into a value between 0 and 1. <norm>
	pow() : Facilitates exponential expressions. <pow>
	round() : Calculates the integer closest to the n parameter. <round>
	sq() : Squares a number (multiplies a number by itself). <sq>
	sqrt() : Calculates the square root of a number. <sqrt>

math
^^^^

.. toctree::
	createVector() : Creates a new p5.Vector (the datatype for storing vectors). <createVector>

noise
^^^^^

.. toctree::
	noise() : Returns the Perlin noise value at specified coordinates. <noise>
	noiseDetail() : Adjusts the character and level of detail produced by the Perlin noise function. <noiseDetail>
	noiseSeed() : Sets the seed value for noise(). <noiseSeed>

p5.Vector
^^^^^^^^^

.. toctree::
	add() : Adds x, y, and z components to a vector, adds one vector to another, or adds two independent vectors together. <add>
	angleBetween() : Calculates and returns the angle (in radians) between two vectors. <angleBetween>
	array() : Return a representation of this vector as a float array. <array>
	copy() : Gets a copy of the vector, returns a p5.Vector object. <copy>
	cross() : Calculates and returns a vector composed of the cross product between two vectors. <cross>
	dist() : Calculates the Euclidean distance between two points (considering a point as a vector object). <dist>
	div() : Divide the vector by a scalar. <div>
	dot() : Calculates the dot product of two vectors. <dot>
	equals() : Equality check against a p5.Vector <equals>
	fromAngle() : Make a new 2D unit vector from an angle <fromAngle>
	heading() : Calculate the angle of rotation for this vector (only 2D vectors) <heading>
	lerp() : Linear interpolate the vector to another vector <lerp>
	limit() : Limit the magnitude of this vector to the value used for the max parameter. <limit>
	mag() : Calculates the magnitude (length) of the vector and returns the result as a float (this is simply the equation sqrt(x*x + y*y + z*z).) <mag>
	magSq() : Calculates the squared magnitude of the vector and returns the result as a float (this is simply the equation (x*x + y*y + z*z).) Faster if the real length is not required in the case of comparing vectors, etc. <magSq>
	mult() : Multiply the vector by a scalar. <mult>
	normalize() : Normalize the vector to length 1 (make it a unit vector). <normalize>
	random2D() : Make a new 2D unit vector from a random angle <random2D>
	random3D() : Make a new random 3D unit vector. <random3D>
	rotate() : Rotate the vector by an angle (only 2D vectors), magnitude remains the same <rotate>
	set() : Sets the x, y, and z component of the vector using two or three separate variables, the data from a p5.Vector, or the values from a float array. <set>
	setMag() : Set the magnitude of this vector to the value used for the len parameter. <setMag>
	sub() : Subtracts x, y, and z components from a vector, subtracts one vector from another, or subtracts two independent vectors. <sub>

random
^^^^^^

.. toctree::
	random() : Return a random floating-point number. <random>
	randomGaussian() : Returns a random number fitting a Gaussian, or normal, distribution. <randomGaussian>
	randomSeed() : Sets the seed value for random(). <randomSeed>

trigonometry
^^^^^^^^^^^^

.. toctree::
	acos() : The inverse of cos(), returns the arc cosine of a value. <acos>
	angleMode() : Sets the current mode of p5 to given mode. <angleMode>
	asin() : The inverse of sin(), returns the arc sine of a value. <asin>
	atan() : The inverse of tan(), returns the arc tangent of a value. <atan>
	atan2() : Calculates the angle (in radians) from a specified point to the coordinate origin as measured from the positive x-axis. <atan2>
	cos() : Calculates the cosine of an angle. <cos>
	degrees() : Converts a radian measurement to its corresponding value in degrees. <degrees>
	radians() : Converts a degree measurement to its corresponding value in radians. <radians>
	sin() : Calculates the sine of an angle. <sin>
	tan() : Calculates the tangent of an angle. <tan>

typography
----------

attributes
^^^^^^^^^^

.. toctree::
	textAlign() : Sets the current alignment for drawing text. <textAlign>
	textAscent() : Returns the ascent of the current font at its current size. <textAscent>
	textDescent() : Returns the descent of the current font at its current size. <textDescent>
	textLeading() : Sets/gets the spacing, in pixels, between lines of text. <textLeading>
	textSize() : Sets/gets the current font size. <textSize>
	textStyle() : Sets/gets the style of the text for system fonts to NORMAL, ITALIC, or BOLD. <textStyle>
	textWidth() : Calculates and returns the width of any character or text string. <textWidth>

loading_displaying
^^^^^^^^^^^^^^^^^^

.. toctree::
	loadFont() : Loads an opentype font file (.otf, .ttf) from a file or a URL, and returns a PFont Object. <loadFont>
	text() : Draws text to the screen. <text>
	textFont() : Sets the current font that will be drawn with the text() function. <textFont>

p5.Font
^^^^^^^

.. toctree::
	textBounds() : Returns a tight bounding box for the given text string using this font (currently only supports single lines) <textBounds>

utilities
---------

array_functions
^^^^^^^^^^^^^^^

.. toctree::
	append() : Adds a value to the end of an array. <append>
	arrayCopy() : Copies an array (or part of an array) to another array. <arrayCopy>
	concat() : Concatenates two arrays, maps to Array.concat(). <concat>
	reverse() : Reverses the order of an array, maps to Array.reverse() <reverse>
	shorten() : Decreases an array by one element and returns the shortened array, maps to Array.pop(). <shorten>
	shuffle() : Randomizes the order of the elements of an array. <shuffle>
	sort() : Sorts an array of numbers from smallest to largest, or puts an array of words in alphabetical order. <sort>
	splice() : Inserts a value or an array of values into an existing array. <splice>
	subset() : Extracts an array of elements from an existing array. <subset>

conversion
^^^^^^^^^^

.. toctree::
	boolean() : Converts a number or string to its boolean representation. <boolean>
	byte() : Converts a number, string or boolean to its byte representation. <byte>
	char() : Converts a number or string to its corresponding single-character string representation. <char>
	float() : Converts a string to its floating point representation. <float>
	hex() : Converts a number to a string in its equivalent hexadecimal notation. <hex>
	int() : Converts a boolean, string, or float to its integer representation. <int>
	str() : Converts a boolean, string or number to its string representation. <str>
	unchar() : Converts a single-character string to its corresponding integer representation. <unchar>
	unhex() : Converts a string representation of a hexadecimal number to its equivalent integer value. <unhex>

string_functions
^^^^^^^^^^^^^^^^

.. toctree::
	join() : Combines an array of Strings into one String, each separated by the character(s) used for the separator parameter. <join>
	match() : This function is used to apply a regular expression to a piece of text, and return matching groups (elements found inside parentheses) as a String array. <match>
	matchAll() : This function is used to apply a regular expression to a piece of text, and return a list of matching groups (elements found inside parentheses) as a two-dimensional String array. <matchAll>
	nf() : Utility function for formatting numbers into strings. <nf>
	nfc() : Utility function for formatting numbers into strings and placing appropriate commas to mark units of 1000. <nfc>
	nfp() : Utility function for formatting numbers into strings. <nfp>
	nfs() : Utility function for formatting numbers into strings. <nfs>
	split() : The split() function maps to String.split(), it breaks a String into pieces using a character or string as the delimiter. <split>
	splitTokens() : The splitTokens() function splits a String at one or many character delimiters or "tokens." The delim parameter specifies the character or characters to be used as a boundary. <splitTokens>
	trim() : Removes whitespace characters from the beginning and end of a String. <trim>

time_date
^^^^^^^^^

.. toctree::
	day() : p5.js communicates with the clock on your computer. <day>
	hour() : p5.js communicates with the clock on your computer. <hour>
	millis() : Returns the number of milliseconds (thousandths of a second) since starting the program. <millis>
	minute() : p5.js communicates with the clock on your computer. <minute>
	month() : p5.js communicates with the clock on your computer. <month>
	second() : p5.js communicates with the clock on your computer. <second>
	year() : p5.js communicates with the clock on your computer. <year>

webgl
-----

camera
^^^^^^

.. toctree::
	camera() : Sets camera position for a 3D sketch. <camera>
	ortho() : Setup ortho camera <ortho>
	perspective() : Sets perspective camera. <perspective>

light
^^^^^

.. toctree::
	ambientLight() : Creates an ambient light with a color <ambientLight>
	directionalLight() : Creates a directional light with a color and a direction <directionalLight>
	pointLight() : Creates a point light with a color and a light position <pointLight>

loading
^^^^^^^

.. toctree::
	loadModel() : Load a 3d model from an OBJ file. <loadModel>
	model() : Render a 3d model to the screen. <model>
	parseObj() : Parse OBJ lines into model. <parseObj>

material
^^^^^^^^

.. toctree::
	ambientMaterial() : Ambient material for geometry with a given color. <ambientMaterial>
	loadShader() : Loads a custom shader from the provided vertex and fragment shader paths. <loadShader>
	normalMaterial() : Normal material for geometry. <normalMaterial>
	shader() : The shader() function lets the user provide a custom shader to fill in shapes in WEBGL mode. <shader>
	specularMaterial() : Specular material for geometry with a given color. <specularMaterial>
	texture() : Texture for geometry. <texture>

p5.Geometry
^^^^^^^^^^^

.. toctree::
	averageNormals() : Averages the vertex normals. <averageNormals>
	averagePoleNormals() : Averages pole normals. <averagePoleNormals>
	computeNormals() : computes smooth normals per vertex as an average of each face. <computeNormals>
	normalize() : Modifies all vertices to be centered within the range -100 to 100. <normalize>

p5.Matrix
^^^^^^^^^

.. toctree::
	copy() : return a copy of a matrix <copy>
	determinant() : inspired by Toji's mat4 determinant <determinant>
	get() : Gets a copy of the vector, returns a p5.Matrix object. <get>
	identity() : return an identity matrix <identity>
	inverseTranspose() : converts a 4x4 matrix to its 3x3 inverse tranform commonly used in MVMatrix to NMatrix conversions. <inverseTranspose>
	invert() : invert  matrix according to a give matrix <invert>
	invert3x3() : Inverts a 3x3 matrix <invert3x3>
	mult() : multiply two mat4s <mult>
	ortho() : sets the ortho matrix <ortho>
	perspective() : sets the perspective matrix <perspective>
	rotate() : rotate our Matrix around an axis by the given angle. <rotate>
	scale() : scales a p5.Matrix by scalars or a vector <scale>
	set() : Sets the x, y, and z component of the vector using two or three separate variables, the data from a p5.Matrix, or the values from a float array. <set>
	translate() :  <translate>
	transpose() : transpose according to a given matrix <transpose>
	transpose3x3() : transposes a 3x3 p5.Matrix by a mat3 <transpose3x3>

p5.RendererGL.Immediate
^^^^^^^^^^^^^^^^^^^^^^^

.. toctree::
	beginShape() : Begin shape drawing. <beginShape>
	endShape() : End shape drawing and render vertices to screen. <endShape>
	vertex() : adds a vertex to be drawn in a custom Shape. <vertex>

p5.RendererGL
^^^^^^^^^^^^^

.. toctree::
	background() : [background description] <background>
	clear() : clears color and depth buffers with r,g,b,a <clear>
	fill() : Basic fill material for geometry with a given color <fill>
	get() : Returns an array of [R,G,B,A] values for any pixel or grabs a section of an image. <get>
	loadPixels() : Loads the pixels data for this canvas into the pixels[] attribute. <loadPixels>
	noFill() : Does not render fill material <noFill>
	noStroke() : Does not render stroke <noStroke>
	pop() : [pop description] <pop>
	push() : pushes a copy of the model view matrix onto the MV Matrix stack. <push>
	resize() : [resize description] <resize>
	scale() : Scales the Model View Matrix by a vector <scale>
	setAttributes() : Set attributes for the WebGL Drawing context. <setAttributes>
	stroke() : Basic stroke material for geometry with a given color <stroke>
	strokeWeight() : Change weight of stroke <strokeWeight>
	translate() : [translate description] <translate>

p5.RendererGL.Retained
^^^^^^^^^^^^^^^^^^^^^^

.. toctree::
	createBuffers() : createBuffers description <createBuffers>
	drawBuffers() : Draws buffers given a geometry key ID <drawBuffers>

p5.Shader
^^^^^^^^^

.. toctree::
	bindShader() : initializes (if needed) and binds the shader program. <bindShader>
	enableAttrib() :  <enableAttrib>
	init() : Creates, compiles, and links the shader based on its sources for the vertex and fragment shaders (provided to the constructor). <init>
	setUniform() : Wrapper around gl.uniform functions. <setUniform>
	unbindShader() :  <unbindShader>
	useProgram() :  <useProgram>

p5.Texture
^^^^^^^^^^

.. toctree::
	bindTexture() : Binds the texture to the appropriate GL target. <bindTexture>
	init() : Initializes common texture parameters, creates a gl texture, tries to upload the texture for the first time if data is already available. <init>
	unbindTexture() : Unbinds the texture from the appropriate GL target. <unbindTexture>
	update() : Checks if the source data for this texture has changed (if it's easy to do so) and reuploads the texture if necessary. <update>

primitives
^^^^^^^^^^

.. toctree::
	box() : Draw a box with given width, height and depth <box>
	cone() : Draw a cone with given radius and height <cone>
	cylinder() : Draw a cylinder with given radius and height <cylinder>
	ellipsoid() : Draw an ellipsoid with given radius <ellipsoid>
	plane() : Draw a plane with given a width and height <plane>
	sphere() : Draw a sphere with given radius <sphere>
	torus() : Draw a torus with given radius and tube radius <torus>

