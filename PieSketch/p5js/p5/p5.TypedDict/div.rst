.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

div()
=====

Divide a value stored at a certain key
The quotient is stored in that location in the Dictionary.

**รูปแบบการใช้งาน**

div ( Key, Amount )

**พารามิเตอร์**

- ``Key``  Number: for value you wish to divide

- ``Amount``  Number: to divide the value by


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var myDictionary = createNumberDict(2, 8);
	  myDictionary.div(2, 2);
	  console.log(myDictionary.get(2)); // logs 4 to console.
	}

	</script>

	<br><br>

.. toctree::

