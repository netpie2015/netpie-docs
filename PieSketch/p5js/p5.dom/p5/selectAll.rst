.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

selectAll()
===========

Searches the page for elements with the given class or tag name (using the '.' prefix
to specify a class and no prefix for a tag) and returns them as p5.Elements
in an array.
The DOM node itself can be accessed with .elt.
Returns an empty array if none found.
You can also specify a container to search within.

**รูปแบบการใช้งาน**

selectAll ( name, [container] )

**พารามิเตอร์**

- ``name``  String: class or tag name of elements to search for

- ``container``  String: id, p5.Element, or HTML element to search within


**ค่าที่ส่งออกมา**

- Array: Array of p5.Elements containing nodes found


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  createButton('btn');
	  createButton('2nd btn');
	  createButton('3rd btn');
	  var buttons = selectAll('button');
	
	  for (var i = 0; i < buttons.length; i++){
	    buttons[i].size(100,100);
	  }
	}
	// these are all valid calls to selectAll()
	var a = selectAll('.moo');
	var b = selectAll('div');
	var c = selectAll('button', '#myContainer');
	var d = select('#container');
	var e = selectAll('p', d);
	var f = document.getElementById('beep');
	var g = select('.blah', f);

	</script>

	<br><br>

.. toctree::

