.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

pRotationY
============

The system variable pRotationY always contains the rotation of the
device along the y axis in the frame previous to the current frame. Value
is represented as 0 to +/-90 degrees.

pRotationY can also be used with rotationY to determine the rotate
direction of the device along the Y-axis.

**รูปแบบการใช้งาน**

pRotationY

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// A simple if statement looking at whether
	// rotationY - pRotationY < 0 is true or not will be
	// sufficient for determining the rotate direction
	// in most cases.
	
	// Some extra logic is needed to account for cases where
	// the angles wrap around.
	var rotateDirection = 'clockwise';
	
	// Simple range conversion to make things simpler.
	// This is not absolutely neccessary but the logic
	// will be different in that case.
	
	var rY = rotationY + 180;
	var pRY = pRotationY + 180;
	
	if ((rY - pRY > 0 && rY - pRY < 270)|| rY - pRY < -270){
	  rotateDirection = 'clockwise';
	} else if (rY - pRY < 0 || rY - pRY > 270){
	  rotateDirection = 'counter-clockwise';
	}

	</script>

	<br><br>

.. toctree::

