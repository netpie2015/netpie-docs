.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

createImg()
===========

Creates an &lt;img&gt; element in the DOM with given src and
alternate text.
Appends to the container node if one is specified, otherwise
appends to body.

**รูปแบบการใช้งาน**

createImg ( src, [alt], [successCallback] )

**พารามิเตอร์**

- ``src``  String: src path or url for image

- ``alt``  String: alternate text to be used if image does not load

- ``successCallback``  function: callback to be called once image data is loaded


**ค่าที่ส่งออกมา**

- Object,p5.Element: pointer to p5.Element holding created node


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var img;
	function setup() {
	  img = createImg('http://p5js.org/img/asterisk-01.png');
	}

	</script>

	<br><br>

.. toctree::

