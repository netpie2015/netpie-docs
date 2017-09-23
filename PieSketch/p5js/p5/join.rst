.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

join()
======

Combines an array of Strings into one String, each separated by the
character(s) used for the separator parameter. To join arrays of ints or
floats, it's necessary to first convert them to Strings using nf() or
nfs().

**รูปแบบการใช้งาน**

join ( list, separator )

**พารามิเตอร์**

- ``list``  : array of Strings to be joined

- ``separator``  : String to be placed between each item


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var array = ["Hello", "world!"]
	var separator = " "
	var message = join(array, separator);
	text(message, 5, 50);
	</script>

	<br><br>

.. toctree::

