.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

loadModel()
===========

Load a 3d model from an OBJ file.

One of the limitations of the OBJ format is that it doesn't have a built-in
sense of scale. This means that models exported from different programs might
be very different sizes. If your model isn't displaying, try calling
loadModel() with the normalized parameter set to true. This will resize the
model to a scale appropriate for p5. You can also make additional changes to
the final size of your model with the scale() function.

**รูปแบบการใช้งาน**

loadModel ( path, normalize, [successCallback], [failureCallback] )

**พารามิเตอร์**

- ``path``  : Path of the model to be loaded

- ``normalize``  : If true, scale the model to a standardized size when loading

- ``successCallback``  : Function to be called once the model is loaded. Will be passed the 3D model object.

- ``failureCallback``  : called with event error if the image fails to load.


.. toctree::

