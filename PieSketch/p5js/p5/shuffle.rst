.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

shuffle()
=========

Randomizes the order of the elements of an array. Implements
<a href="http://Bost.Ocks.org/mike/shuffle/" target=_blank>
Fisher-Yates Shuffle Algorithm</a>.

**รูปแบบการใช้งาน**

shuffle ( array, [bool] )

**พารามิเตอร์**

- ``array``  : Array to shuffle

- ``bool``  : modify passed array


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var regularArr = ['ABC', 'def', createVector(), TAU, Math.E];
	  print(regularArr);
	  shuffle(regularArr, true); // force modifications to passed array
	  print(regularArr);
	
	  // By default shuffle() returns a shuffled cloned array:
	  var newArr = shuffle(regularArr);
	  print(regularArr);
	  print(newArr);
	}
	</script>

	<br><br>

.. toctree::

