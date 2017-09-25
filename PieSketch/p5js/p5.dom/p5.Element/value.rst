.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

value()
=======

Either returns the value of the element if no arguments
given, or sets the value of the element.

**รูปแบบการใช้งาน**

value ( [value] )

**พารามิเตอร์**

- ``value``  String,Number: 


**ค่าที่ส่งออกมา**

- String,Object,p5.Element: value of element if no value is specified or p5.Element


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// gets the value
	var inp;
	function setup() {
	  inp = createInput('');
	}
	
	function mousePressed() {
	  print(inp.value());
	}
	// sets the value
	var inp;
	function setup() {
	  inp = createInput('myValue');
	}
	
	function mousePressed() {
	  inp.value("myValue");
	}

	</script>

	<br><br>

.. toctree::

