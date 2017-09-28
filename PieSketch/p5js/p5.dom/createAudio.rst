.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

createAudio()
=============

สร้างองค์ประกอบ HTML5  ที่ซ่อนไว้ใน DOM เพื่อการเล่นเสียงที่เรียบง่าย ผนวกเข้ากับโหนดคอนเทนเนอร์หากมีการระบุไว้มิฉะนั้นจะต่อท้ายกับเนื้อหา พารามิเตอร์ตัวแรกอาจเป็นเส้นทางสตริงเดี่ยวไปยังไฟล์เสียงหรืออาร์เรย์ของเส้นทางสตริงไปยังรูปแบบต่างๆของเสียงเดียวกัน วิธีนี้มีประโยชน์ในการทำให้มั่นใจว่าเสียงของคุณสามารถเล่นผ่านเบราว์เซอร์ต่างๆได้เนื่องจากแต่ละรูปแบบจะสนับสนุนรูปแบบต่างๆ ดู หน้านี้สำหรับข้อมูลเพิ่มเติมเกี่ยวกับรูปแบบที่สนับสนุน

.. Creates a hidden HTML5 &lt;audio&gt; element in the DOM for simple audio
.. playback. Appends to the container node if one is specified,
.. otherwise appends to body. The first parameter
.. can be either a single string path to a audio file, or an array of string
.. paths to different formats of the same audio. This is useful for ensuring
.. that your audio can play across different browsers, as each supports
.. different formats. See this
.. page for further information about supported formats.

**รูปแบบการใช้งาน**

createAudio ( src, [callback] )

**พารามิเตอร์**

- ``src``  String,Array: เส้นทางไปยังไฟล์เสียงหรืออาร์เรย์ของเส้นทางสำหรับการสนับสนุนเบราว์เซอร์ที่แตกต่างกัน

- ``callback``  Object: ฟังก์ชันเรียกกลับจะถูกเรียกใช้เมื่อเกิดไฟเหตุการณ์ &#39;canplaythrough&#39; นั่นคือเมื่อเบราว์เซอร์สามารถเล่นสื่อและคาดว่ามีการโหลดข้อมูลที่เพียงพอในการเล่นสื่อจนจบโดยไม่ต้องหยุดการเก็บเนื้อหาเพิ่มเติม

.. ``src``  String,Array: path to an audio file, or array of paths for supporting different browsers
.. ``callback``  Object: callback function to be called upon 'canplaythrough' event fire, that is, when the browser can play the media, and estimates that enough data has been loaded to play the media up to its end without having to stop for further buffering of content

**ค่าที่ส่งออกมา**

- p5.MediaElement,p5.Element: ชี้ไปยังเสียง p5.Element

.. p5.MediaElement,p5.Element: pointer to audio p5.Element

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
