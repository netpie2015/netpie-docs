.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

print()
=======

The print() function writes to the console area of your browser.
This function is often helpful for looking at the data a program is
producing. This function creates a new line of text for each call to
the function. Individual elements can be
separated with quotes ("") and joined with the addition operator (+).

While print() is similar to console.log(), it does not directly map to
it in order to simulate easier to understand behavior than
console.log(). Due to this, it is slower. For fastest results, use
console.log().

**รูปแบบการใช้งาน**

print ( contents )

**พารามิเตอร์**

- ``contents``  Any: any combination of Number, String, Object, Boolean, Array to print


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	<code class='norender'>
	var x = 10;
	print("The value of x is " + x);
	// prints "The value of x is 10"


	</script>

	<br><br>

.. toctree::

