.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

frameRate()
===========

ระบุจำนวนเฟรมที่จะแสดงทุกวินาที ตัวอย่างเช่นเฟรมการเรียกฟังก์ชัน Rate (30) จะพยายามรีเฟรช 30 ครั้งต่อวินาที หากโปรเซสเซอร์ไม่เร็วพอที่จะรักษาอัตราที่กำหนดอัตราเฟรมจะไม่สามารถทำได้ แนะนำให้ตั้งค่าอัตราเฟรมภายในการตั้งค่า () อัตราการผิดนัดคือ 60 เฟรมต่อวินาที นี่เป็นเช่นเดียวกับ setFrameRate (val) 
การเรียก frameRate () ที่ไม่มีอาร์กิวเมนต์จะส่งกลับเฟรมเรตปัจจุบัน ฟังก์ชันการวาดต้องทำงานอย่างน้อยหนึ่งครั้งก่อนที่จะส่งคืนค่า นี่เป็นเช่นเดียวกับ getFrameRate () 
การเรียก frameRate () ที่มีอาร์กิวเมนต์ที่ไม่ใช่ตัวเลขประเภทหรือไม่เป็นบวกจะส่งกลับเฟรมปัจจุบันด้วย

.. Specifies the number of frames to be displayed every second. For example,
.. the function call frameRate(30) will attempt to refresh 30 times a second.
.. If the processor is not fast enough to maintain the specified rate, the
.. frame rate will not be achieved. Setting the frame rate within setup() is
.. recommended. The default rate is 60 frames per second. This is the same as
.. setFrameRate(val).
.. 
.. Calling frameRate() with no arguments returns the current framerate. The
.. draw function must run at least once before it will return a value. This
.. is the same as getFrameRate().
.. 
.. Calling frameRate() with arguments that are not of the type numbers
.. or are non positive also returns current framerate.

**รูปแบบการใช้งาน**

frameRate ( fps )

**พารามิเตอร์**

- ``fps``  Number: จำนวนเฟรมที่จะแสดงทุกวินาที

.. ``fps``  Number: number of frames to be displayed every second

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
