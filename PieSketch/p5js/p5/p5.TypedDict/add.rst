.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

add()
=====

Add to a value stored at a certain key
The sum is stored in that location in the Dictionary.

**รูปแบบการใช้งาน**

add ( Key, Amount )

**พารามิเตอร์**

- ``Key``  Number: for value you wish to add to

- ``Amount``  Number: to add to the value


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var myDictionary = createNumberDict(2, 5);
	  myDictionary.add(2, 2);
	  console.log(myDictionary.get(2)); // logs 7 to console.
	}

	</script>

	<br><br>

.. toctree::

