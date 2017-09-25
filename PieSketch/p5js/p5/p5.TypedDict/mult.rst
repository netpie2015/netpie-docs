.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

mult()
======

Multiply a value stored at a certain key
The product is stored in that location in the Dictionary.

**รูปแบบการใช้งาน**

mult ( Key, Amount )

**พารามิเตอร์**

- ``Key``  Number: for value you wish to multiply

- ``Amount``  Number: to multiply the value by


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var myDictionary = createNumberDict(2, 4);
	  myDictionary.mult(2, 2);
	  console.log(myDictionary.get(2)); // logs 8 to console.
	}

	</script>

	<br><br>

.. toctree::

