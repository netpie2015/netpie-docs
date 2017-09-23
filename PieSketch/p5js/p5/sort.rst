.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

sort()
======

Sorts an array of numbers from smallest to largest, or puts an array of
words in alphabetical order. The original array is not modified; a
re-ordered array is returned. The count parameter states the number of
elements to sort. For example, if there are 12 elements in an array and
count is set to 5, only the first 5 elements in the array will be sorted.

**รูปแบบการใช้งาน**

sort ( list, [count] )

**พารามิเตอร์**

- ``list``  : Array to sort

- ``count``  : number of elements to sort, starting from 0


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var words = new Array("banana", "apple", "pear","lime");
	  print(words); // ["banana", "apple", "pear", "lime"]
	  var count = 4; // length of array
	
	  words = sort(words, count);
	  print(words); // ["apple", "banana", "lime", "pear"]
	}
	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var numbers = new Array(2,6,1,5,14,9,8,12);
	  print(numbers); // [2,6,1,5,14,9,8,12]
	  var count = 5; // Less than the length of the array
	
	  numbers = sort(numbers, count);
	  print(numbers); // [1,2,5,6,14,9,8,12]
	}
	</script>

	<br><br>

.. toctree::

