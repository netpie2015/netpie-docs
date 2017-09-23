.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

beginShape()
============

Begin shape drawing.  This is a helpful way of generating
custom shapes quickly.  However in WEBGL mode, application
performance will likely drop as a result of too many calls to
beginShape() / endShape().  As a high performance alternative,
please use p5.js geometry primitives.

**รูปแบบการใช้งาน**

beginShape ( mode )

**พารามิเตอร์**

- ``mode``  : webgl primitives mode. beginShape supports the following modes: POINTS,LINES,LINE_STRIP,LINE_LOOP,TRIANGLES, TRIANGLE_STRIP,and TRIANGLE_FAN.


.. toctree::

