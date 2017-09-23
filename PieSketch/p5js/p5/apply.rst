.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

apply()
=======

Applys a filter function to a canvas.
The difference between this and the actual filter functions defined below
is that the filter functions generally modify the pixel buffer but do
not actually put that data back to the canvas (where it would actually
update what is visible). By contrast this method does make the changes
actually visible in the canvas.
The apply method is the method that callers of this module would generally
use. It has been separated from the actual filters to support an advanced
use case of creating a filter chain that executes without actually updating
the canvas in between everystep.

**รูปแบบการใช้งาน**

apply ( canvas, func, filterParam )

**พารามิเตอร์**

- ``canvas``  : [description]

- ``func``  : [description]

- ``filterParam``  : [description]


.. toctree::

