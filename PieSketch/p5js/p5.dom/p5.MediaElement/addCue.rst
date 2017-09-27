.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

addCue()
========

กำหนดเวลากิจกรรมเพื่อเรียกใช้ทุกครั้งที่ MediaElement (เสียง / วิดีโอ) ถึงจุดคิวการเล่น ยอมรับฟังก์ชันการโทรกลับเวลา (เป็นวินาที) ที่จะเรียกใช้การโทรกลับและพารามิเตอร์ที่เป็นตัวเลือกสำหรับการโทรกลับ เวลาจะถูกส่งผ่านไปเป็นพารามิเตอร์แรกในฟังก์ชัน callback และ param จะเป็นพารามิเตอร์ที่สอง

.. Schedule events to trigger every time a MediaElement
..  (audio/video) reaches a playback cue point.
..  Accepts a callback function, a time (in seconds) at which to trigger
..  the callback, and an optional parameter for the callback.
..  Time will be passed as the first parameter to the callback function,
..  and param will be the second parameter.

**รูปแบบการใช้งาน**

addCue ( time, callback, [value] )

**พารามิเตอร์**

- ``time``  Number: เวลาเป็นวินาทีเทียบกับการเล่นขององค์ประกอบสื่อนี้ ตัวอย่างเช่นเมื่อต้องการเรียกใช้เหตุการณ์ทุกครั้งที่การเล่นถึงสองวินาทีให้ส่งผ่านไปยังหมายเลข 2 ซึ่งจะถูกส่งผ่านไปเป็นพารามิเตอร์แรกในฟังก์ชันการเรียกกลับ

- ``callback``  function: ชื่อของฟังก์ชันที่จะถูกเรียกในเวลาที่กำหนด การเรียกกลับจะได้รับเวลาและ param (optionally) เป็นพารามิเตอร์สองตัว

- ``value``  Object: วัตถุที่จะถูกส่งผ่านไปเป็นพารามิเตอร์ที่สองให้กับฟังก์ชัน callback

.. ``time``  Number: Time in seconds, relative to this media element's playback. For example, to trigger an event every time playback reaches two seconds, pass in the number 2. This will be passed as the first parameter to the callback function.
.. ``callback``  function: Name of a function that will be called at the given time. The callback will receive time and (optionally) param as its two parameters.
.. ``value``  Object: An object to be passed as the second parameter to the callback function.

**ค่าที่ส่งออกมา**

- Number: id ID ของคิวนี้มีประโยชน์สำหรับ removeCue (id)

.. Number: id ID of this cue, useful for removeCue(id)

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

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
