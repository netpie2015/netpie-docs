.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

onended()
=========

กำหนดเวลากิจกรรมที่จะเรียกเมื่อองค์ประกอบเสียงหรือวิดีโอถึงจุดสิ้นสุด หากองค์ประกอบกำลังวนลูปจะไม่มีการเรียกใช้ องค์ประกอบถูกส่งผ่านไปเป็นอาร์กิวเมนต์ที่เรียกใช้การเรียกกลับ

.. Schedule an event to be called when the audio or video
..  element reaches the end. If the element is looping,
..  this will not be called. The element is passed in
..  as the argument to the onended callback.

**รูปแบบการใช้งาน**

onended ( callback )

**พารามิเตอร์**

- ``callback``  function: ฟังก์ชั่นการโทรเมื่อ soundfile สิ้นสุดลง องค์ประกอบสื่อจะถูกส่งผ่านไปเป็นอาร์กิวเมนต์สำหรับการโทรกลับ

.. ``callback``  function: function to call when the soundfile has ended. The media element will be passed in as the argument to the callback.

**ค่าที่ส่งออกมา**

- Object,p5.MediaElement: 

.. Object,p5.MediaElement: 

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

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
