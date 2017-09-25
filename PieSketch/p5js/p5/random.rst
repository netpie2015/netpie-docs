.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

random()
========

Return a random floating-point number.
Takes either 0, 1 or 2 arguments.
If no argument is given, returns a random number from 0
up to (but not including) 1.
If one argument is given and it is a number, returns a random number from 0
up to (but not including) the number.
If one argument is given and it is an array, returns a random element from
that array.
If two arguments are given, returns a random number from the
first argument up to (but not including) the second argument.

**รูปแบบการใช้งาน**

random ( [min], [max] )

**พารามิเตอร์**

- ``min``  Number: the lower bound (inclusive)

- ``max``  Number: the upper bound (exclusive)


**ค่าที่ส่งออกมา**

- Number: the random number


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	for (var i = 0; i < 100; i++) {
	  var r = random(50);
	  stroke(r*5);
	  line(50, i, 50+r, i);
	}

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	for (var i = 0; i < 100; i++) {
	  var r = random(-50, 50);
	  line(50,i,50+r,i);
	}

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Get a random element from an array using the random(Array) syntax
	var words = [ "apple", "bear", "cat", "dog" ];
	var word = random(words);  // select random word
	text(word,10,50);  // draw the word

	</script>

	<br><br>

.. toctree::

