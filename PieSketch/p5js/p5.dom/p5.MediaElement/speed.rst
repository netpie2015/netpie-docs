.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

speed()
=======

หากไม่ได้รับอาร์กิวเมนต์ให้ส่งคืนความเร็วในการเล่นในปัจจุบันขององค์ประกอบ พารามิเตอร์ความเร็วกำหนดความเร็วที่ 2.0 จะเล่นองค์ประกอบสองครั้งเร็ว 0.5 จะเล่นที่ความเร็วครึ่งหนึ่งและ -1 จะเล่นองค์ประกอบในความเร็วปกติในการย้อนกลับ (โปรดทราบว่าเบราว์เซอร์ไม่สนับสนุนการเล่นย้อนหลังและแม้ว่าจะมี การเล่นอาจไม่ราบรื่น)

.. If no arguments are given, returns the current playback speed of the
.. element. The speed parameter sets the speed where 2.0 will play the
.. element twice as fast, 0.5 will play at half the speed, and -1 will play
.. the element in normal speed in reverse.(Note that not all browsers support
.. backward playback and even if they do, playback might not be smooth.)

**รูปแบบการใช้งาน**

speed ( [speed] )

**พารามิเตอร์**

- ``speed``  Number: speed สำหรับการเล่นองค์ประกอบ

.. ``speed``  Number: speed multiplier for element playback

**ค่าที่ส่งออกมา**

- Number,Object,p5.MediaElement: ความเร็วในการเล่นปัจจุบันหรือ p5.MediaElement

.. Number,Object,p5.MediaElement: current playback speed or p5.MediaElement

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
