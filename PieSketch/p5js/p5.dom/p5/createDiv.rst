.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

createDiv()
===========

Creates a &lt;div&gt;&lt;/div&gt; element in the DOM with given inner HTML.
Appends to the container node if one is specified, otherwise
appends to body.

**รูปแบบการใช้งาน**

createDiv ( [html] )

**พารามิเตอร์**

- ``html``  String: inner HTML for element created


**ค่าที่ส่งออกมา**

- Object,p5.Element: pointer to p5.Element holding created node


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var myDiv;
	function setup() {
	  myDiv = createDiv('this is some text');
	}

	</script>

	<br><br>

.. toctree::

