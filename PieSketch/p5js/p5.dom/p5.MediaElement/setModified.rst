.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

setModified()
=============

helper method for web GL mode to indicate that an element has been
changed or unchanged since last upload. gl texture upload will
set this value to false after uploading the texture; or might set
it to true if metadata has become available but there is no actual
texture data available yet..

**รูปแบบการใช้งาน**

setModified ( val )

**พารามิเตอร์**

- ``val``  boolean: sets whether or not the element has been modified.


.. toctree::

