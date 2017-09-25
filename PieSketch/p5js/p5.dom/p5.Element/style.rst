.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

style()
=======

Sets the given style (css) property (1st arg) of the element with the
given value (2nd arg). If a single argument is given, .style()
returns the value of the given property; however, if the single argument
is given in css syntax ('text-align:center'), .style() sets the css
appropriatly. .style() also handles 2d and 3d css transforms. If
the 1st arg is 'rotate', 'translate', or 'position', the following arguments
accept Numbers as values. ('translate', 10, 100, 50);

**รูปแบบการใช้งาน**

style ( property, [value] )

**พารามิเตอร์**

- ``property``  String: property to be set

- ``value``  String,Number,p5.Color: value to assign to property (only String|Number for rotate/translate)


**ค่าที่ส่งออกมา**

- String,Object,p5.Element: value of property, if no value is specified or p5.Element


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	<code class="norender">
	var myDiv = createDiv("I like pandas.");
	myDiv.style("font-size", "18px");
	myDiv.style("color", "#ff0000");
	<code class="norender">
	var col = color(25,23,200,50);
	var button = createButton("button");
	button.style("background-color", col);
	button.position(10, 10);
	<code class="norender">
	var myDiv = createDiv("I like lizards.");
	myDiv.style("position", 20, 20);
	myDiv.style("rotate", 45);
	<code class="norender">
	var myDiv;
	function setup() {
	  background(200);
	  myDiv = createDiv("I like gray.");
	  myDiv.position(20, 20);
	}
	
	function draw() {
	  myDiv.style("font-size", mouseX+"px");
	}

	</script>

	<br><br>

.. toctree::

