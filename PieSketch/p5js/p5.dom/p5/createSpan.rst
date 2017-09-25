.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

createSpan()
============

Creates a &lt;span&gt;&lt;/span&gt; element in the DOM with given inner HTML.
Appends to the container node if one is specified, otherwise
appends to body.

**รูปแบบการใช้งาน**

createSpan ( [html] )

**พารามิเตอร์**

- ``html``  String: inner HTML for element created


**ค่าที่ส่งออกมา**

- Object,p5.Element: pointer to p5.Element holding created node


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var mySpan;
	function setup() {
	  mySpan = createSpan('this is some text');
	}

	</script>

	<br><br>

.. toctree::

