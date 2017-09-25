.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

createButton()
==============

Creates a &lt;button&gt;&lt;/button&gt; element in the DOM.
Use .size() to set the display size of the button.
Use .mousePressed() to specify behavior on press.
Appends to the container node if one is specified, otherwise
appends to body.

**รูปแบบการใช้งาน**

createButton ( label, [value] )

**พารามิเตอร์**

- ``label``  String: label displayed on the button

- ``value``  String: value of the button


**ค่าที่ส่งออกมา**

- Object,p5.Element: pointer to p5.Element holding created node


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var button;
	function setup() {
	  createCanvas(100, 100);
	  background(0);
	  button = createButton('click me');
	  button.position(19, 19);
	  button.mousePressed(changeBG);
	}
	
	function changeBG() {
	  var val = random(255);
	  background(val);
	}

	</script>

	<br><br>

.. toctree::

