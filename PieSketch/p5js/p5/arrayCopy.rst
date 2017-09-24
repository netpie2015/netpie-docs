.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

arrayCopy()
===========

Copies an array (or part of an array) to another array. The src array is
copied to the dst array, beginning at the position specified by
srcPosition and into the position specified by dstPosition. The number of
elements to copy is determined by length. Note that copying values
overwrites existing values in the destination array. To append values
instead of overwriting them, use concat().

The simplified version with only two arguments, arrayCopy(src, dst),
copies an entire array to another of the same size. It is equivalent to
arrayCopy(src, 0, dst, 0, src.length).

Using this function is far more efficient for copying array data than
iterating through a for() loop and copying each element individually.

**รูปแบบการใช้งาน**

arrayCopy ( src, srcPosition, dst, dstPosition, length )

**พารามิเตอร์**

- ``src``  Array: the source Array

- ``srcPosition``  Number: starting position in the source Array

- ``dst``  Array: the destination Array

- ``dstPosition``  Number: starting position in the destination Array

- ``length``  Number: number of Array elements to be copied


.. toctree::

