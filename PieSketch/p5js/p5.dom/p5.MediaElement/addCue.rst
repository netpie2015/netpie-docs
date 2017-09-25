.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

addCue()
========

Schedule events to trigger every time a MediaElement
 (audio/video) reaches a playback cue point.
 Accepts a callback function, a time (in seconds) at which to trigger
 the callback, and an optional parameter for the callback.
 Time will be passed as the first parameter to the callback function,
 and param will be the second parameter.

**รูปแบบการใช้งาน**

addCue ( time, callback, [value] )

**พารามิเตอร์**

- ``time``  Number: Time in seconds, relative to this media element's playback. For example, to trigger an event every time playback reaches two seconds, pass in the number 2. This will be passed as the first parameter to the callback function.

- ``callback``  function: Name of a function that will be called at the given time. The callback will receive time and (optionally) param as its two parameters.

- ``value``  Object: An object to be passed as the second parameter to the callback function.


**ค่าที่ส่งออกมา**

- Number: id ID of this cue, useful for removeCue(id)


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	 function setup() {
	   background(255,255,255);
	
	   audioEl = createAudio('assets/beat.mp3');
	   audioEl.showControls();
	
	   // schedule three calls to changeBackground
	   audioEl.addCue(0.5, changeBackground, color(255,0,0) );
	   audioEl.addCue(1.0, changeBackground, color(0,255,0) );
	   audioEl.addCue(2.5, changeBackground, color(0,0,255) );
	   audioEl.addCue(3.0, changeBackground, color(0,255,255) );
	   audioEl.addCue(4.2, changeBackground, color(255,255,0) );
	   audioEl.addCue(5.0, changeBackground, color(255,255,0) );
	 }
	
	 function changeBackground(val) {
	   background(val);
	 }
	 

	</script>

	<br><br>

.. toctree::

