.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

curveTightness()
================

Modifies the quality of forms created with curve() and curveVertex().
The parameter tightness determines how the curve fits to the vertex
points. The value 0.0 is the default value for tightness (this value
defines the curves to be Catmull-Rom splines) and the value 1.0 connects
all the points with straight lines. Values within the range -5.0 and 5.0
will deform the curves but will leave them recognizable and as values
increase in magnitude, they will continue to deform.

**รูปแบบการใช้งาน**

curveTightness ( amount )

**พารามิเตอร์**

- ``amount``  Number: of deformation from the original vertices


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Move the mouse left and right to see the curve change
	
	function setup() {
	  createCanvas(100, 100);
	  noFill();
	}
	
	function draw() {
	  background(204);
	  var t = map(mouseX, 0, width, -5, 5);
	  curveTightness(t);
	  beginShape();
	  curveVertex(10, 26);
	  curveVertex(10, 26);
	  curveVertex(83, 24);
	  curveVertex(83, 61);
	  curveVertex(25, 65);
	  curveVertex(25, 65);
	  endShape();
	}


	</script>

	<br><br>

.. toctree::

