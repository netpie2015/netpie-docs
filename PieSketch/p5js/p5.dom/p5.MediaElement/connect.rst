.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

connect()
=========

ส่งเอาต์พุตเสียงของอิลิเมนต์นี้ไปยังออบเจ็กต์ audioNode หรือ p5.sound ที่ระบุ หากไม่มีองค์ประกอบใดให้เชื่อมต่อกับเอาต์พุตหลักของ p5 การเชื่อมต่อดังกล่าวถูกสร้างขึ้นเมื่อใช้วิธีนี้เป็นครั้งแรก การเชื่อมต่อทั้งหมดจะถูกเอาออกโดยใช้. disconnect () method วิธีนี้ใช้เพื่อใช้กับห้องสมุด addon p5.sound.js

.. Send the audio output of this element to a specified audioNode or
..  p5.sound object. If no element is provided, connects to p5's master
..  output. That connection is established when this method is first called.
..  All connections are removed by the .disconnect() method.
..  This method is meant to be used with the p5.sound.js addon library.

**รูปแบบการใช้งาน**

connect ( audioNode )

**พารามิเตอร์**

- ``audioNode``  AudioNode,Object: AudioNode จาก Web Audio API หรือวัตถุจากไลบรารี p5.sound

.. ``audioNode``  AudioNode,Object: AudioNode from the Web Audio API, or an object from the p5.sound library

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
