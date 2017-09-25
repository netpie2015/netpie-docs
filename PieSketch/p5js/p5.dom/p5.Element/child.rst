.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

child()
=======

Attaches the element  as a child to the parent specified.
Accepts either a string ID, DOM node, or p5.Element.
If no argument is specified, an array of children DOM nodes is returned.

**รูปแบบการใช้งาน**

child ( [child] )

**พารามิเตอร์**

- ``child``  String,Object,p5.Element: the ID, DOM node, or p5.Element to add to the current element


**ค่าที่ส่งออกมา**

- p5.Element: 


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var div0 = createDiv('this is the parent');
	var div1 = createDiv('this is the child');
	div0.child(div1); // use p5.Element
	var div0 = createDiv('this is the parent');
	var div1 = createDiv('this is the child');
	div1.id('apples');
	div0.child('apples'); // use id
	var div0 = createDiv('this is the parent');
	var elt = document.getElementById('myChildDiv');
	div0.child(elt); // use element from page

	</script>

	<br><br>

.. toctree::

