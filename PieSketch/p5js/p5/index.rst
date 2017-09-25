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

constants
^^^^^^^^^

.. toctree::
	ADD :  <ADD>
	BASELINE :  <BASELINE>
	BEVEL :  <BEVEL>
	BLEND :  <BLEND>
	BLUR :  <BLUR>
	BOLD :  <BOLD>
	BOTTOM :  <BOTTOM>
	BURN :  <BURN>
	CENTER :  <CENTER>
	CHORD :  <CHORD>
	CLOSE :  <CLOSE>
	CORNER :  <CORNER>
	CORNERS :  <CORNERS>
	DARKEST :  <DARKEST>
	DEGREES :  <DEGREES>
	DIFFERENCE :  <DIFFERENCE>
	DILATE :  <DILATE>
	DODGE :  <DODGE>
	ERODE :  <ERODE>
	EXCLUSION :  <EXCLUSION>
	GRAY :  <GRAY>
	HALF_PI : HALF_PI is a mathematical constant with the value 1.57079632679489661923. <HALF_PI>
	HARD_LIGHT :  <HARD_LIGHT>
	HSB :  <HSB>
	HSL :  <HSL>
	INVERT :  <INVERT>
	ITALIC :  <ITALIC>
	LANDSCAPE :  <LANDSCAPE>
	LEFT :  <LEFT>
	LIGHTEST :  <LIGHTEST>
	LINES :  <LINES>
	LINE_LOOP :  <LINE_LOOP>
	LINE_STRIP :  <LINE_STRIP>
	MITER :  <MITER>
	MULTIPLY :  <MULTIPLY>
	NORMAL :  <NORMAL>
	OPAQUE :  <OPAQUE>
	OPEN :  <OPEN>
	OVERLAY :  <OVERLAY>
	P2D :  <P2D>
	PI : PI is a mathematical constant with the value 3.14159265358979323846. <PI>
	PIE :  <PIE>
	POINTS :  <POINTS>
	PORTRAIT :  <PORTRAIT>
	POSTERIZE :  <POSTERIZE>
	PROJECT :  <PROJECT>
	QUADS :  <QUADS>
	QUAD_STRIP :  <QUAD_STRIP>
	QUARTER_PI : QUARTER_PI is a mathematical constant with the value 0.7853982. <QUARTER_PI>
	RADIANS :  <RADIANS>
	RADIUS :  <RADIUS>
	REPLACE :  <REPLACE>
	RGB :  <RGB>
	RIGHT :  <RIGHT>
	ROUND :  <ROUND>
	SCREEN :  <SCREEN>
	SOFT_LIGHT :  <SOFT_LIGHT>
	SQUARE :  <SQUARE>
	TAU : TAU is an alias for TWO_PI, a mathematical constant with the value 6.28318530717958647693. <TAU>
	THRESHOLD :  <THRESHOLD>
	TOP :  <TOP>
	TRIANGLES :  <TRIANGLES>
	TRIANGLE_FAN :  <TRIANGLE_FAN>
	TRIANGLE_STRIP :  <TRIANGLE_STRIP>
	TWO_PI : TWO_PI is a mathematical constant with the value 6.28318530717958647693. <TWO_PI>
	WEBGL :  <WEBGL>

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
	displayHeight : System variable that stores the height of the entire screen display. <displayHeight>
	displayWidth : System variable that stores the width of the entire screen display. <displayWidth>
	focused : Confirms if the window a p5.js program is in is "focused," meaning that the sketch will accept mouse or keyboard input. <focused>
	frameCount : The system variable frameCount contains the number of frames that have been displayed since the program started. <frameCount>
	frameRate() : Specifies the number of frames to be displayed every second. <frameRate>
	fullscreen() : If argument is given, sets the sketch to fullscreen or not based on the value of the argument. <fullscreen>
	getFrameRate() : Returns the current framerate. <getFrameRate>
	getURL() : Gets the current URL. <getURL>
	getURLParams() : Gets the current URL params as an Object. <getURLParams>
	getURLPath() : Gets the current URL path as an array. <getURLPath>
	height : System variable that stores the height of the drawing canvas. <height>
	noCursor() : Hides the cursor from view. <noCursor>
	pixelDensity() : Sets the pixel scaling for high pixel density displays. <pixelDensity>
	print() : The print() function writes to the console area of your browser. <print>
	setFrameRate() : Specifies the number of frames to be displayed every second. <setFrameRate>
	width : System variable that stores the width of the drawing canvas. <width>
	windowHeight : System variable that stores the height of the inner window, it maps to window.innerHeight. <windowHeight>
	windowResized() : The windowResized() function is called once every time the browser window is resized. <windowResized>
	windowWidth : System variable that stores the width of the inner window, it maps to window.innerWidth. <windowWidth>

p5.Element
^^^^^^^^^^

.. toctree::
	changed() : The .changed() function is called when the value of an element is changed. <p5.Element/changed>
	class() : Adds given class to the element. <p5.Element/class>
	doubleClicked() : The .doubleClicked() function is called once after every time a mouse button is pressed twice over the element. <p5.Element/doubleClicked>
	dragLeave() : The .dragLeave() function is called once after every time a dragged file leaves the element area. <p5.Element/dragLeave>
	dragOver() : The .dragOver() function is called once after every time a file is dragged over the element. <p5.Element/dragOver>
	drop() : The .drop() function is called for each file dropped on the element. <p5.Element/drop>
	elt : Underlying HTML element. <p5.Element/elt>
	id() : Sets the ID of the element. <p5.Element/id>
	input() : The .input() function is called when any user input is detected with an element. <p5.Element/input>
	mouseClicked() : The .mouseClicked() function is called once after a mouse button is pressed and released over the element. <p5.Element/mouseClicked>
	mouseMoved() : The .mouseMoved() function is called once every time a mouse moves over the element. <p5.Element/mouseMoved>
	mouseOut() : The .mouseOut() function is called once after every time a mouse moves off the element. <p5.Element/mouseOut>
	mouseOver() : The .mouseOver() function is called once after every time a mouse moves onto the element. <p5.Element/mouseOver>
	mousePressed() : The .mousePressed() function is called once after every time a mouse button is pressed over the element. <p5.Element/mousePressed>
	mouseReleased() : The .mouseReleased() function is called once after every time a mouse button is released over the element. <p5.Element/mouseReleased>
	mouseWheel() : The .mouseWheel() function is called once after every time a mouse wheel is scrolled over the element. <p5.Element/mouseWheel>
	parent() : Attaches the element to the parent specified. <p5.Element/parent>
	touchEnded() : The .touchEnded() function is called once after every time a touch is registered. <p5.Element/touchEnded>
	touchMoved() : The .touchMoved() function is called once after every time a touch move is registered. <p5.Element/touchMoved>
	touchStarted() : The .touchStarted() function is called once after every time a touch is registered. <p5.Element/touchStarted>

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
	add() : Add to a value stored at a certain key The sum is stored in that location in the Dictionary. <p5.TypedDict/add>
	clear() : Empties Dictionary of all key-value pairs <p5.TypedDict/clear>
	create() : Removes a key-value pair in the Dictionary <p5.TypedDict/create>
	createNumberDict() : Creates a new instance of p5.NumberDict using the key, value pair or object you provide. <p5.TypedDict/createNumberDict>
	createStringDict() : Creates a new instance of p5.StringDict using the key, value pair or object you provide. <p5.TypedDict/createStringDict>
	div() : Divide a value stored at a certain key The quotient is stored in that location in the Dictionary. <p5.TypedDict/div>
	get() : Returns value stored at supplied key. <p5.TypedDict/get>
	hasKey() : Returns true if key exists in Dictionary otherwise returns false <p5.TypedDict/hasKey>
	maxKey() : Return the highest key. <p5.TypedDict/maxKey>
	maxValue() : Return the highest value. <p5.TypedDict/maxValue>
	minKey() : Return the lowest key. <p5.TypedDict/minKey>
	minValue() : Return the lowest value. <p5.TypedDict/minValue>
	mult() : Multiply a value stored at a certain key The product is stored in that location in the Dictionary. <p5.TypedDict/mult>
	print() : Logs the list of items currently in the Dictionary to the console <p5.TypedDict/print>
	remove() : Removes a key-value pair in the Dictionary <p5.TypedDict/remove>
	saveJSON() : Converts the Dictionary into a JSON file for local storage. <p5.TypedDict/saveJSON>
	saveTable() : Converts the Dictionary into a CSV file for local storage. <p5.TypedDict/saveTable>
	set() : Changes the value of key if in it already exists in in the Dictionary otherwise makes a new key-value pair <p5.TypedDict/set>
	size() : Returns the number of key-value pairs currently in Dictionary object <p5.TypedDict/size>
	sub() : Subtract from a value stored at a certain key The difference is stored in that location in the Dictionary. <p5.TypedDict/sub>

events
------

acceleration
^^^^^^^^^^^^

.. toctree::
	accelerationX : The system variable accelerationX always contains the acceleration of the device along the x axis. <accelerationX>
	accelerationY : The system variable accelerationY always contains the acceleration of the device along the y axis. <accelerationY>
	accelerationZ : The system variable accelerationZ always contains the acceleration of the device along the z axis. <accelerationZ>
	deviceMoved() : The deviceMoved() function is called when the device is moved by more than the threshold value along X, Y or Z axis. <deviceMoved>
	deviceOrientation : The system variable deviceOrientation always contains the orientation of the device. <deviceOrientation>
	deviceShaken() : The deviceShaken() function is called when the device total acceleration changes of accelerationX and accelerationY values is more than the threshold value. <deviceShaken>
	deviceTurned() : The deviceTurned() function is called when the device rotates by more than 90 degrees continuously. <deviceTurned>
	pAccelerationX : The system variable pAccelerationX always contains the acceleration of the device along the x axis in the frame previous to the current frame. <pAccelerationX>
	pAccelerationY : The system variable pAccelerationY always contains the acceleration of the device along the y axis in the frame previous to the current frame. <pAccelerationY>
	pAccelerationZ : The system variable pAccelerationZ always contains the acceleration of the device along the z axis in the frame previous to the current frame. <pAccelerationZ>
	pRotationX : The system variable pRotationX always contains the rotation of the device along the x axis in the frame previous to the current frame. <pRotationX>
	pRotationY : The system variable pRotationY always contains the rotation of the device along the y axis in the frame previous to the current frame. <pRotationY>
	pRotationZ : The system variable pRotationZ always contains the rotation of the device along the z axis in the frame previous to the current frame. <pRotationZ>
	rotationX : The system variable rotationX always contains the rotation of the device along the x axis. <rotationX>
	rotationY : The system variable rotationY always contains the rotation of the device along the y axis. <rotationY>
	rotationZ : The system variable rotationZ always contains the rotation of the device along the z axis. <rotationZ>
	setMoveThreshold() : The setMoveThreshold() function is used to set the movement threshold for the deviceMoved() function. <setMoveThreshold>
	setShakeThreshold() : The setShakeThreshold() function is used to set the movement threshold for the deviceShaken() function. <setShakeThreshold>

keyboard
^^^^^^^^

.. toctree::
	areDownKeys() : The checkDownKeys function returns a boolean true if any keys pressed and a false if no keys are currently pressed. <areDownKeys>
	downKeys : Holds the key codes of currently pressed keys. <downKeys>
	isKeyPressed : The boolean system variable keyIsPressed is true if any key is pressed and false if no keys are pressed. <isKeyPressed>
	key : The system variable key always contains the value of the most recent key on the keyboard that was typed. <key>
	keyCode : The variable keyCode is used to detect special keys such as BACKSPACE, DELETE, ENTER, RETURN, TAB, ESCAPE, SHIFT, CONTROL, OPTION, ALT, UP_ARROW, DOWN_ARROW, LEFT_ARROW, RIGHT_ARROW. <keyCode>
	keyIsDown() : The keyIsDown() function checks if the key is currently down, i.e. <keyIsDown>
	keyPressed() : The keyPressed() function is called once every time a key is pressed. <keyPressed>
	keyReleased() : The keyReleased() function is called once every time a key is released. <keyReleased>
	keyTyped() : The keyTyped() function is called once every time a key is pressed, but action keys such as Ctrl, Shift, and Alt are ignored. <keyTyped>

mouse
^^^^^

.. toctree::
	doubleClicked() : The doubleClicked() function is executed every time a event listener has detected a dblclick event which is a part of the DOM L3 specification. <doubleClicked>
	mouseButton : Processing automatically tracks if the mouse button is pressed and which button is pressed. <mouseButton>
	mouseClicked() : The mouseClicked() function is called once after a mouse button has been pressed and then released. <mouseClicked>
	mouseDragged() : The mouseDragged() function is called once every time the mouse moves and a mouse button is pressed. <mouseDragged>
	mouseIsPressed : The boolean system variable mouseIsPressed is true if the mouse is pressed and false if not. <mouseIsPressed>
	mouseMoved() : The mouseMoved() function is called every time the mouse moves and a mouse button is not pressed. <mouseMoved>
	mousePressed() : The mousePressed() function is called once after every time a mouse button is pressed. <mousePressed>
	mouseReleased() : The mouseReleased() function is called every time a mouse button is released. <mouseReleased>
	mouseWheel() : The function mouseWheel() is executed every time a vertical mouse wheel event is detected either triggered by an actual mouse wheel or by a touchpad. <mouseWheel>
	mouseX : The system variable mouseX always contains the current horizontal position of the mouse, relative to (0, 0) of the canvas. <mouseX>
	mouseY : The system variable mouseY always contains the current vertical position of the mouse, relative to (0, 0) of the canvas. <mouseY>
	pmouseX : The system variable pmouseX always contains the horizontal position of the mouse or finger in the frame previous to the current frame, relative to (0, 0) of the canvas. <pmouseX>
	pmouseY : The system variable pmouseY always contains the vertical position of the mouse or finger in the frame previous to the current frame, relative to (0, 0) of the canvas. <pmouseY>
	pwinMouseX : The system variable pwinMouseX always contains the horizontal position of the mouse in the frame previous to the current frame, relative to (0, 0) of the window. <pwinMouseX>
	pwinMouseY : The system variable pwinMouseY always contains the vertical position of the mouse in the frame previous to the current frame, relative to (0, 0) of the window. <pwinMouseY>
	winMouseX : The system variable winMouseX always contains the current horizontal position of the mouse, relative to (0, 0) of the window. <winMouseX>
	winMouseY : The system variable winMouseY always contains the current vertical position of the mouse, relative to (0, 0) of the window. <winMouseY>

touch
^^^^^

.. toctree::
	touchEnded() : The touchEnded() function is called every time a touch ends. <touchEnded>
	touchMoved() : The touchMoved() function is called every time a touch move is registered. <touchMoved>
	touchStarted() : The touchStarted() function is called once after every time a touch is registered. <touchStarted>
	touches : The system variable touches[] contains an array of the positions of all current touch points, relative to (0, 0) of the canvas, and IDs identifying a unique touch as it moves. <touches>

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
	blend() : Copies a region of pixels from one image to another, using a specified blend mode to do the operation. <p5.Image/blend>
	copy() : Copies a region of pixels from one image to another. <p5.Image/copy>
	filter() : Applies an image filter to a p5.Image <p5.Image/filter>
	get() : Get a region of pixels from an image. <p5.Image/get>
	height : Image height. <p5.Image/height>
	isModified() : helper method for web GL mode to figure out if the image has been modified and might need to be re-uploaded to texture memory between frames. <p5.Image/isModified>
	loadPixels() : Loads the pixels data for this image into the [pixels] attribute. <p5.Image/loadPixels>
	mask() : Masks part of an image from displaying by loading another image and using it's alpha channel as an alpha channel for this image. <p5.Image/mask>
	pixels : Array containing the values for all the pixels in the display window. <p5.Image/pixels>
	resize() : Resize the image to a new width and height. <p5.Image/resize>
	save() : Saves the image to a file and force the browser to download it. <p5.Image/save>
	set() : Set the color of a single pixel or write an image into this p5.Image. <p5.Image/set>
	setModified() : helper method for web GL mode to indicate that an image has been changed or unchanged since last upload. <p5.Image/setModified>
	updatePixels() : Updates the backing canvas for this image with the contents of the [pixels] array. <p5.Image/updatePixels>
	width : Image width. <p5.Image/width>

pixels
^^^^^^

.. toctree::
	blend() : Copies a region of pixels from one image to another, using a specified blend mode to do the operation. <blend>
	copy() : Copies a region of the canvas to another region of the canvas and copies a region of pixels from an image used as the srcImg parameter into the canvas srcImage is specified this is used as the source. <copy>
	filter() : Applies a filter to the canvas. <filter>
	get() : Returns an array of [R,G,B,A] values for any pixel or grabs a section of an image. <get>
	loadPixels() : Loads the pixel data for the display window into the pixels[] array. <loadPixels>
	pixels : Uint8ClampedArray containing the values for all the pixels in the display window. <pixels>
	set() : Changes the color of any pixel, or writes an image directly to the display window. <set>
	updatePixels() : Updates the display window with the data in the pixels[] array. <updatePixels>

io
--

files
^^^^^

.. toctree::
	destroyClickedElement() : Helper function, a callback for download that deletes  an invisible anchor element from the DOM once the file  has been automatically downloaded. <destroyClickedElement>
	downloadFile() : Forces download. <downloadFile>
	httpDo() : Method for executing an HTTP request. <httpDo>
	httpGet() : Method for executing an HTTP GET request. <httpGet>
	httpPost() : Method for executing an HTTP POST request. <httpPost>
	loadJSON() : Loads a JSON file from a file or a URL, and returns an Object or Array. <loadJSON>
	loadStrings() : Reads the contents of a file and creates a String array of its individual lines. <loadStrings>
	loadTable() : Reads the contents of a file or URL and creates a p5.Table object with its values. <loadTable>
	loadXML() : Reads the contents of a file and creates an XML object with its values. <loadXML>
	save() : Save an image, text, json, csv, wav, or html. <save>
	saveJSON() : Writes the contents of an Array or a JSON object to a .json file. <saveJSON>
	saveStrings() : Writes an array of Strings to a text file, one line per String. <saveStrings>
	saveTable() : Writes the contents of a Table object to a file. <saveTable>
	writeFile() : Generate a blob of file data as a url to prepare for download. <writeFile>

p5.Table
^^^^^^^^

.. toctree::
	addColumn() : Use addColumn() to add a new column to a Table object. <p5.Table/addColumn>
	addRow() : Use addRow() to add a new row of data to a p5.Table object. <p5.Table/addRow>
	clearRows() : Removes all rows from a Table. <p5.Table/clearRows>
	columns :  <p5.Table/columns>
	findRow() : Finds the first row in the Table that contains the value  provided, and returns a reference to that row. <p5.Table/findRow>
	findRows() : Finds the rows in the Table that contain the value  provided, and returns references to those rows. <p5.Table/findRows>
	get() : Retrieves a value from the Table's specified row and column. <p5.Table/get>
	getArray() : Retrieves all table data and returns it as a multidimensional array. <p5.Table/getArray>
	getColumn() : Retrieves all values in the specified column, and returns them  as an array. <p5.Table/getColumn>
	getNum() : Retrieves a Float value from the Table's specified row and column. <p5.Table/getNum>
	getObject() : Retrieves all table data and returns as an object. <p5.Table/getObject>
	getRow() : Returns a reference to the specified p5.TableRow. <p5.Table/getRow>
	getRowCount() : Returns the total number of rows in a Table. <p5.Table/getRowCount>
	getRows() : Gets all rows from the table. <p5.Table/getRows>
	getString() : Retrieves a String value from the Table's specified row and column. <p5.Table/getString>
	matchRow() : Finds the first row in the Table that matches the regular  expression provided, and returns a reference to that row. <p5.Table/matchRow>
	matchRows() : Finds the rows in the Table that match the regular expression provided,  and returns references to those rows. <p5.Table/matchRows>
	removeColumn() : Use removeColumn() to remove an existing column from a Table  object. <p5.Table/removeColumn>
	removeRow() : Removes a row from the table object. <p5.Table/removeRow>
	removeTokens() : Removes any of the specified characters (or "tokens"). <p5.Table/removeTokens>
	rows :  <p5.Table/rows>
	set() : Stores a value in the Table's specified row and column. <p5.Table/set>
	setNum() : Stores a Float value in the Table's specified row and column. <p5.Table/setNum>
	setString() : Stores a String value in the Table's specified row and column. <p5.Table/setString>
	trim() : Trims leading and trailing whitespace, such as spaces and tabs,  from String table values. <p5.Table/trim>

p5.TableRow
^^^^^^^^^^^

.. toctree::
	get() : Retrieves a value from the TableRow's specified column. <p5.TableRow/get>
	getNum() : Retrieves a Float value from the TableRow's specified  column. <p5.TableRow/getNum>
	getString() : Retrieves an String value from the TableRow's specified  column. <p5.TableRow/getString>
	set() : Stores a value in the TableRow's specified column. <p5.TableRow/set>
	setNum() : Stores a Float value in the TableRow's specified column. <p5.TableRow/setNum>
	setString() : Stores a String value in the TableRow's specified column. <p5.TableRow/setString>

p5.XML
^^^^^^

.. toctree::
	addChild() : Appends a new child to the element. <p5.XML/addChild>
	getAttributeCount() : Counts the specified element's number of attributes, returned as an Number. <p5.XML/getAttributeCount>
	getChild() : Returns the first of the element's children that matches the name parameter or the child of the given index.It returns undefined if no matching child is found. <p5.XML/getChild>
	getChildren() : Returns all of the element's children as an array of p5.XML objects. <p5.XML/getChildren>
	getContent() : Returns the content of an element. <p5.XML/getContent>
	getName() : Gets the element's full name, which is returned as a String. <p5.XML/getName>
	getNum() : Returns an attribute value of the element as an Number. <p5.XML/getNum>
	getParent() : Gets a copy of the element's parent. <p5.XML/getParent>
	getString() : Returns an attribute value of the element as an String. <p5.XML/getString>
	hasAttribute() : Checks whether or not an element has the specified attribute. <p5.XML/hasAttribute>
	hasChildren() : Checks whether or not the element has any children, and returns the result as a boolean. <p5.XML/hasChildren>
	listAttributes() : Gets all of the specified element's attributes, and returns them as an array of Strings. <p5.XML/listAttributes>
	listChildren() : Get the names of all of the element's children, and returns the names as an array of Strings. <p5.XML/listChildren>
	removeChild() : Removes the element specified by name or index. <p5.XML/removeChild>
	setAttribute() : Sets the content of an element's attribute. <p5.XML/setAttribute>
	setContent() : Sets the element's content. <p5.XML/setContent>
	setName() : Sets the element's name, which is specified as a String. <p5.XML/setName>

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

noise
^^^^^

.. toctree::
	noise() : Returns the Perlin noise value at specified coordinates. <noise>
	noiseDetail() : Adjusts the character and level of detail produced by the Perlin noise function. <noiseDetail>
	noiseSeed() : Sets the seed value for noise(). <noiseSeed>

p5.Vector
^^^^^^^^^

.. toctree::
	add() : Adds x, y, and z components to a vector, adds one vector to another, or adds two independent vectors together. <p5.Vector/add>
	angleBetween() : Calculates and returns the angle (in radians) between two vectors. <p5.Vector/angleBetween>
	array() : Return a representation of this vector as a float array. <p5.Vector/array>
	copy() : Gets a copy of the vector, returns a p5.Vector object. <p5.Vector/copy>
	cross() : Calculates and returns a vector composed of the cross product between two vectors. <p5.Vector/cross>
	dist() : Calculates the Euclidean distance between two points (considering a point as a vector object). <p5.Vector/dist>
	div() : Divide the vector by a scalar. <p5.Vector/div>
	dot() : Calculates the dot product of two vectors. <p5.Vector/dot>
	equals() : Equality check against a p5.Vector <p5.Vector/equals>
	fromAngle() : Make a new 2D unit vector from an angle <p5.Vector/fromAngle>
	heading() : Calculate the angle of rotation for this vector (only 2D vectors) <p5.Vector/heading>
	lerp() : Linear interpolate the vector to another vector <p5.Vector/lerp>
	limit() : Limit the magnitude of this vector to the value used for the max parameter. <p5.Vector/limit>
	mag() : Calculates the magnitude (length) of the vector and returns the result as a float (this is simply the equation sqrt(x*x + y*y + z*z).) <p5.Vector/mag>
	magSq() : Calculates the squared magnitude of the vector and returns the result as a float (this is simply the equation (x*x + y*y + z*z).) Faster if the real length is not required in the case of comparing vectors, etc. <p5.Vector/magSq>
	mult() : Multiply the vector by a scalar. <p5.Vector/mult>
	normalize() : Normalize the vector to length 1 (make it a unit vector). <p5.Vector/normalize>
	random2D() : Make a new 2D unit vector from a random angle <p5.Vector/random2D>
	random3D() : Make a new random 3D unit vector. <p5.Vector/random3D>
	rotate() : Rotate the vector by an angle (only 2D vectors), magnitude remains the same <p5.Vector/rotate>
	set() : Sets the x, y, and z component of the vector using two or three separate variables, the data from a p5.Vector, or the values from a float array. <p5.Vector/set>
	setMag() : Set the magnitude of this vector to the value used for the len parameter. <p5.Vector/setMag>
	sub() : Subtracts x, y, and z components from a vector, subtracts one vector from another, or subtracts two independent vectors. <p5.Vector/sub>
	x : The x component of the vector <p5.Vector/x>
	y : The y component of the vector <p5.Vector/y>
	z : The z component of the vector <p5.Vector/z>

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
	font : Underlying opentype font implementation <p5.Font/font>
	textBounds() : Returns a tight bounding box for the given text string using this font (currently only supports single lines) <p5.Font/textBounds>

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
	averageNormals() : Averages the vertex normals. <p5.Geometry/averageNormals>
	averagePoleNormals() : Averages pole normals. <p5.Geometry/averagePoleNormals>
	computeNormals() : computes smooth normals per vertex as an average of each face. <p5.Geometry/computeNormals>
	normalize() : Modifies all vertices to be centered within the range -100 to 100. <p5.Geometry/normalize>

p5.Matrix
^^^^^^^^^

.. toctree::
	copy() : return a copy of a matrix <p5.Matrix/copy>
	determinant() : inspired by Toji's mat4 determinant <p5.Matrix/determinant>
	exports : PRIVATE <p5.Matrix/exports>
	get() : Gets a copy of the vector, returns a p5.Matrix object. <p5.Matrix/get>
	identity() : return an identity matrix <p5.Matrix/identity>
	inverseTranspose() : converts a 4x4 matrix to its 3x3 inverse tranform commonly used in MVMatrix to NMatrix conversions. <p5.Matrix/inverseTranspose>
	invert() : invert  matrix according to a give matrix <p5.Matrix/invert>
	invert3x3() : Inverts a 3x3 matrix <p5.Matrix/invert3x3>
	mult() : multiply two mat4s <p5.Matrix/mult>
	ortho() : sets the ortho matrix <p5.Matrix/ortho>
	perspective() : sets the perspective matrix <p5.Matrix/perspective>
	rotate() : rotate our Matrix around an axis by the given angle. <p5.Matrix/rotate>
	scale() : scales a p5.Matrix by scalars or a vector <p5.Matrix/scale>
	set() : Sets the x, y, and z component of the vector using two or three separate variables, the data from a p5.Matrix, or the values from a float array. <p5.Matrix/set>
	translate() :  <p5.Matrix/translate>
	transpose() : transpose according to a given matrix <p5.Matrix/transpose>
	transpose3x3() : transposes a 3x3 p5.Matrix by a mat3 <p5.Matrix/transpose3x3>

p5.RendererGL.Immediate
^^^^^^^^^^^^^^^^^^^^^^^

.. toctree::
	beginShape() : Begin shape drawing. <p5.RendererGL.Immediate/beginShape>
	endShape() : End shape drawing and render vertices to screen. <p5.RendererGL.Immediate/endShape>
	vertex() : adds a vertex to be drawn in a custom Shape. <p5.RendererGL.Immediate/vertex>

p5.RendererGL
^^^^^^^^^^^^^

.. toctree::
	background() : [background description] <p5.RendererGL/background>
	clear() : clears color and depth buffers with r,g,b,a <p5.RendererGL/clear>
	fill() : Basic fill material for geometry with a given color <p5.RendererGL/fill>
	get() : Returns an array of [R,G,B,A] values for any pixel or grabs a section of an image. <p5.RendererGL/get>
	loadPixels() : Loads the pixels data for this canvas into the pixels[] attribute. <p5.RendererGL/loadPixels>
	noFill() : Does not render fill material <p5.RendererGL/noFill>
	noStroke() : Does not render stroke <p5.RendererGL/noStroke>
	pop() : [pop description] <p5.RendererGL/pop>
	push() : pushes a copy of the model view matrix onto the MV Matrix stack. <p5.RendererGL/push>
	resize() : [resize description] <p5.RendererGL/resize>
	scale() : Scales the Model View Matrix by a vector <p5.RendererGL/scale>
	setAttributes() : Set attributes for the WebGL Drawing context. <p5.RendererGL/setAttributes>
	stroke() : Basic stroke material for geometry with a given color <p5.RendererGL/stroke>
	strokeWeight() : Change weight of stroke <p5.RendererGL/strokeWeight>
	translate() : [translate description] <p5.RendererGL/translate>
	uMVMatrix : model view, projection, & normal matrices <p5.RendererGL/uMVMatrix>

p5.RendererGL.Retained
^^^^^^^^^^^^^^^^^^^^^^

.. toctree::
	createBuffers() : createBuffers description <p5.RendererGL.Retained/createBuffers>
	drawBuffers() : Draws buffers given a geometry key ID <p5.RendererGL.Retained/drawBuffers>

p5.Shader
^^^^^^^^^

.. toctree::
	bindShader() : initializes (if needed) and binds the shader program. <p5.Shader/bindShader>
	enableAttrib() :  <p5.Shader/enableAttrib>
	init() : Creates, compiles, and links the shader based on its sources for the vertex and fragment shaders (provided to the constructor). <p5.Shader/init>
	setUniform() : Wrapper around gl.uniform functions. <p5.Shader/setUniform>
	unbindShader() :  <p5.Shader/unbindShader>
	useProgram() :  <p5.Shader/useProgram>

p5.Texture
^^^^^^^^^^

.. toctree::
	bindTexture() : Binds the texture to the appropriate GL target. <p5.Texture/bindTexture>
	init() : Initializes common texture parameters, creates a gl texture, tries to upload the texture for the first time if data is already available. <p5.Texture/init>
	unbindTexture() : Unbinds the texture from the appropriate GL target. <p5.Texture/unbindTexture>
	update() : Checks if the source data for this texture has changed (if it's easy to do so) and reuploads the texture if necessary. <p5.Texture/update>

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

