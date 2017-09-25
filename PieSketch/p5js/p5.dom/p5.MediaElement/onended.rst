.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

onended()
=========

Schedule an event to be called when the audio or video
 element reaches the end. If the element is looping,
 this will not be called. The element is passed in
 as the argument to the onended callback.

**รูปแบบการใช้งาน**

onended ( callback )

**พารามิเตอร์**

- ``callback``  function: function to call when the soundfile has ended. The media element will be passed in as the argument to the callback.


**ค่าที่ส่งออกมา**

- Object,p5.MediaElement: 


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	 function setup() {
	   audioEl = createAudio('assets/beat.mp3');
	   audioEl.showControls(true);
	   audioEl.onended(sayDone);
	 }
	
	 function sayDone(elt) {
	   alert('done playing ' + elt.src );
	 }
	 

	</script>

	<br><br>

.. toctree::

