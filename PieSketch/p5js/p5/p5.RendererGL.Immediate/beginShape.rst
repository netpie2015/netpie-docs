.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

beginShape()
============

เริ่มวาดรูป นี่เป็นวิธีที่มีประโยชน์ในการสร้างรูปร่างที่กำหนดเองได้อย่างรวดเร็ว อย่างไรก็ตามในโหมด WEBGL ประสิทธิภาพการทำงานของแอพพลิเคชั่นอาจลดลงเนื่องจากมีสายมากเกินไปที่จะเริ่มต้น Shape () / endShape () เป็นทางเลือกที่มีประสิทธิภาพสูงโปรดใช้ primitive geometry primitives ของ p5.js

.. Begin shape drawing.  This is a helpful way of generating
.. custom shapes quickly.  However in WEBGL mode, application
.. performance will likely drop as a result of too many calls to
.. beginShape() / endShape().  As a high performance alternative,
.. please use p5.js geometry primitives.

**รูปแบบการใช้งาน**

beginShape ( mode )

**พารามิเตอร์**

- ``mode``  Number: โหมด primitives ของ webgl beginShape สนับสนุนโหมดต่อไปนี้: POINTS, LINES, LINE_STRIP, LINE_LOOP, TRIANGLES, TRIANGLE_STRIP และ TRIANGLE_FAN

.. ``mode``  Number: webgl primitives mode. beginShape supports the following modes: POINTS,LINES,LINE_STRIP,LINE_LOOP,TRIANGLES, TRIANGLE_STRIP,and TRIANGLE_FAN.

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
