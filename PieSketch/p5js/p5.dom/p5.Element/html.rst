.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

html()
======

If an argument is given, sets the inner HTML of the element,
replacing any existing html. If true is included as a second
argument, html is appended instead of replacing existing html.
If no arguments are given, returns
the inner HTML of the element.

**รูปแบบการใช้งาน**

html ( [html], [append] )

**พารามิเตอร์**

- ``html``  String: the HTML to be placed inside the element

- ``append``  boolean: whether to append HTML to existing


**ค่าที่ส่งออกมา**

- Object,p5.Element,String: 


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var div = createDiv('').size(100,100);
	div.html('hi');
	var div = createDiv('Hello ').size(100,100);
	div.html('World', true);

	</script>

	<br><br>

.. toctree::

