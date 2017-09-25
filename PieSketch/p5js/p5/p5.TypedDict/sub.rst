.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

sub()
=====

Subtract from a value stored at a certain key
The difference is stored in that location in the Dictionary.

**รูปแบบการใช้งาน**

sub ( Key, Amount )

**พารามิเตอร์**

- ``Key``  Number: for value you wish to subtract from

- ``Amount``  Number: to subtract from the value


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var myDictionary = createNumberDict(2, 5);
	  myDictionary.sub(2, 2);
	  console.log(myDictionary.get(2)); // logs 3 to console.
	}

	</script>

	<br><br>

.. toctree::

