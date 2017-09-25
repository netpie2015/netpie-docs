.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

center()
========

Centers a p5 Element either vertically, horizontally,
or both, relative to its parent or according to
the body if the Element has no parent. If no argument is passed
the Element is aligned both vertically and horizontally.

**รูปแบบการใช้งาน**

center ( align )

**พารามิเตอร์**

- ``align``  String: passing 'vertical', 'horizontal' aligns element accordingly


**ค่าที่ส่งออกมา**

- Object,p5.Element: pointer to p5.Element


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var div = createDiv('').size(10,10);
	  div.style('background-color','orange');
	  div.center();
	
	}

	</script>

	<br><br>

.. toctree::

