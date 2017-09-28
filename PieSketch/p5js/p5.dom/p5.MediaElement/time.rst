.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

time()
======

หากไม่ได้รับอาร์กิวเมนต์ให้ส่งคืนเวลาปัจจุบันของอิลิเมนต์ ถ้ามีอาร์กิวเมนต์ระบุเวลาปัจจุบันของอิลิเมนต์ถูกตั้งค่าไว้

.. If no arguments are given, returns the current time of the element.
.. If an argument is given the current time of the element is set to it.

**รูปแบบการใช้งาน**

time ( [time] )

**พารามิเตอร์**

- ``time``  Number: เวลาที่จะข้ามไป (วินาที)

.. ``time``  Number: time to jump to (in seconds)

**ค่าที่ส่งออกมา**

- Number,Object,p5.MediaElement: เวลาปัจจุบัน (เป็นวินาที) หรือ p5.MediaElement

.. Number,Object,p5.MediaElement: current time (in seconds) or p5.MediaElement

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
