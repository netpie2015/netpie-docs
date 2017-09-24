.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

frameRate()
===========

Specifies the number of frames to be displayed every second. For example,
the function call frameRate(30) will attempt to refresh 30 times a second.
If the processor is not fast enough to maintain the specified rate, the
frame rate will not be achieved. Setting the frame rate within setup() is
recommended. The default rate is 60 frames per second. This is the same as
setFrameRate(val).

Calling frameRate() with no arguments returns the current framerate. The
draw function must run at least once before it will return a value. This
is the same as getFrameRate().

Calling frameRate() with arguments that are not of the type numbers
or are non positive also returns current framerate.

**รูปแบบการใช้งาน**

frameRate ( fps )

**พารามิเตอร์**

- ``fps``  Number: number of frames to be displayed every second


.. toctree::

