.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

connect()
=========

Send the audio output of this element to a specified audioNode or
 p5.sound object. If no element is provided, connects to p5's master
 output. That connection is established when this method is first called.
 All connections are removed by the .disconnect() method.
 This method is meant to be used with the p5.sound.js addon library.

**รูปแบบการใช้งาน**

connect ( audioNode )

**พารามิเตอร์**

- ``audioNode``  AudioNode,Object: AudioNode from the Web Audio API, or an object from the p5.sound library


.. toctree::

