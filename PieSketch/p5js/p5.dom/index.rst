.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

p5
==

p5.dom
------

p5
^^

.. toctree::
	VIDEO : CAMERA STUFF <p5/VIDEO>
	addElement() : Helpers for create methods. <p5/addElement>
	createA() : Creates an &lt;a&gt;&lt;/a&gt; element in the DOM for including a hyperlink. <p5/createA>
	createAudio() : Creates a hidden HTML5 &lt;audio&gt; element in the DOM for simple audio playback. <p5/createAudio>
	createButton() : Creates a &lt;button&gt;&lt;/button&gt; element in the DOM. <p5/createButton>
	createCapture() : Creates a new &lt;video&gt; element that contains the audio/video feed from a webcam. <p5/createCapture>
	createCheckbox() : Creates a checkbox &lt;input&gt;&lt;/input&gt; element in the DOM. <p5/createCheckbox>
	createDiv() : Creates a &lt;div&gt;&lt;/div&gt; element in the DOM with given inner HTML. <p5/createDiv>
	createElement() : Creates element with given tag in the DOM with given content. <p5/createElement>
	createFileInput() : Creates an &lt;input&gt;&lt;/input&gt; element in the DOM of type 'file'. <p5/createFileInput>
	createImg() : Creates an &lt;img&gt; element in the DOM with given src and alternate text. <p5/createImg>
	createInput() : Creates an &lt;input&gt;&lt;/input&gt; element in the DOM for text input. <p5/createInput>
	createMedia() : VIDEO STUFF <p5/createMedia>
	createP() : Creates a &lt;p&gt;&lt;/p&gt; element in the DOM with given inner HTML. <p5/createP>
	createRadio() : Creates a radio button &lt;input&gt;&lt;/input&gt; element in the DOM. <p5/createRadio>
	createSelect() : Creates a dropdown menu &lt;select&gt;&lt;/select&gt; element in the DOM. <p5/createSelect>
	createSlider() : Creates a slider &lt;input&gt;&lt;/input&gt; element in the DOM. <p5/createSlider>
	createSpan() : Creates a &lt;span&gt;&lt;/span&gt; element in the DOM with given inner HTML. <p5/createSpan>
	createVideo() : Creates an HTML5 &lt;video&gt; element in the DOM for simple playback of audio/video. <p5/createVideo>
	getContainer() : Helper function for select and selectAll <p5/getContainer>
	removeElements() : Removes all elements created by p5, except any canvas / graphics elements created by createCanvas or createGraphics. <p5/removeElements>
	select() : Searches the page for an element with the given ID, class, or tag name (using the '#' or '.' prefixes to specify an ID or class respectively, and none for a tag) and returns it as a p5.Element. <p5/select>
	selectAll() : Searches the page for elements with the given class or tag name (using the '.' prefix to specify a class and no prefix for a tag) and returns them as p5.Elements in an array. <p5/selectAll>
	wrapElement() : Helper function for getElement and getElements. <p5/wrapElement>

p5.Element
^^^^^^^^^^

.. toctree::
	addClass() : Adds specified class to the element. <p5.Element/addClass>
	attribute() : Adds a new attribute or changes the value of an existing attribute on the specified element. <p5.Element/attribute>
	center() : Centers a p5 Element either vertically, horizontally, or both, relative to its parent or according to the body if the Element has no parent. <p5.Element/center>
	child() : Attaches the element  as a child to the parent specified. <p5.Element/child>
	hide() : Hides the current element. <p5.Element/hide>
	html() : If an argument is given, sets the inner HTML of the element, replacing any existing html. <p5.Element/html>
	position() : Sets the position of the element relative to (0, 0) of the window. <p5.Element/position>
	remove() : Removes the element and deregisters all listeners. <p5.Element/remove>
	removeAttribute() : Removes an attribute on the specified element. <p5.Element/removeAttribute>
	removeClass() : Removes specified class from the element. <p5.Element/removeClass>
	show() : Shows the current element. <p5.Element/show>
	size() : Sets the width and height of the element. <p5.Element/size>
	style() : Sets the given style (css) property (1st arg) of the element with the given value (2nd arg). <p5.Element/style>
	value() : Either returns the value of the element if no arguments given, or sets the value of the element. <p5.Element/value>

p5.MediaElement
^^^^^^^^^^^^^^^

.. toctree::
	addCue() : Schedule events to trigger every time a MediaElement  (audio/video) reaches a playback cue point. <p5.MediaElement/addCue>
	autoplay() : Set HTML5 media element to autoplay or not. <p5.MediaElement/autoplay>
	clearCues() : Remove all of the callbacks that had originally been scheduled  via the addCue method. <p5.MediaElement/clearCues>
	connect() : Send the audio output of this element to a specified audioNode or  p5.sound object. <p5.MediaElement/connect>
	disconnect() : Disconnect all Web Audio routing, including to master output. <p5.MediaElement/disconnect>
	duration() : Returns the duration of the HTML5 media element. <p5.MediaElement/duration>
	hideControls() : Hide the default mediaElement controls. <p5.MediaElement/hideControls>
	isModified() : helper method for web GL mode to figure out if the element has been modified and might need to be re-uploaded to texture memory between frames. <p5.MediaElement/isModified>
	loop() : Set 'loop' to true for an HTML5 media element, and starts playing. <p5.MediaElement/loop>
	noLoop() : Set 'loop' to false for an HTML5 media element. <p5.MediaElement/noLoop>
	onended() : Schedule an event to be called when the audio or video  element reaches the end. <p5.MediaElement/onended>
	pause() : Pauses an HTML5 media element. <p5.MediaElement/pause>
	play() : Play an HTML5 media element. <p5.MediaElement/play>
	removeCue() : Remove a callback based on its ID. <p5.MediaElement/removeCue>
	setModified() : helper method for web GL mode to indicate that an element has been changed or unchanged since last upload. <p5.MediaElement/setModified>
	showControls() : Show the default MediaElement controls, as determined by the web browser. <p5.MediaElement/showControls>
	speed() : If no arguments are given, returns the current playback speed of the element. <p5.MediaElement/speed>
	stop() : Stops an HTML5 media element (sets current time to zero). <p5.MediaElement/stop>
	time() : If no arguments are given, returns the current time of the element. <p5.MediaElement/time>
	volume() : Sets volume for this HTML5 media element. <p5.MediaElement/volume>

p5.File
^^^^^^^

.. toctree::
	data : URL string containing image data. <p5.File/data>
	file : Underlying File object. <p5.File/file>
	name : File name <p5.File/name>
	size : File size <p5.File/size>
	subtype : File subtype (usually the file extension jpg, png, xml, etc.) <p5.File/subtype>
	type : File type (image, text, etc.) <p5.File/type>

