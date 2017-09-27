.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

createVideo()
=============

สร้างองค์ประกอบ  HTML5 ใน DOM เพื่อการเล่นเสียง / วิดีโอที่เรียบง่าย แสดงโดยค่าเริ่มต้นสามารถซ่อนด้วย. hide () และวาดลงในผืนผ้าใบโดยใช้วิดีโอ () ผนวกเข้ากับโหนดคอนเทนเนอร์หากมีการระบุไว้มิฉะนั้นจะต่อท้ายกับเนื้อหา พารามิเตอร์แรกอาจเป็นเส้นทางสตริงเดี่ยวไปยังไฟล์วิดีโอหรืออาร์เรย์ของเส้นทางสตริงไปยังรูปแบบต่างๆของวิดีโอเดียวกัน วิธีนี้มีประโยชน์ในการทำให้วิดีโอของคุณสามารถเล่นผ่านเบราว์เซอร์ต่างๆเนื่องจากแต่ละรูปแบบจะรองรับรูปแบบต่างๆ ดู หน้านี้ สำหรับข้อมูลเพิ่มเติมเกี่ยวกับรูปแบบที่สนับสนุน

.. Creates an HTML5 &lt;video&gt; element in the DOM for simple playback
.. of audio/video. Shown by default, can be hidden with .hide()
.. and drawn into canvas using video(). Appends to the container
.. node if one is specified, otherwise appends to body. The first parameter
.. can be either a single string path to a video file, or an array of string
.. paths to different formats of the same video. This is useful for ensuring
.. that your video can play across different browsers, as each supports
.. different formats. See this
.. page for further information about supported formats.

**รูปแบบการใช้งาน**

createVideo ( src, [callback] )

**พารามิเตอร์**

- ``src``  String,Array: เส้นทางไปยังไฟล์วิดีโอหรืออาร์เรย์ของพา ธ สำหรับการสนับสนุนเบราว์เซอร์ต่างๆ

- ``callback``  Object: ฟังก์ชันเรียกกลับจะถูกเรียกเมื่อไฟเหตุการณ์ &#39;canplaythrough&#39; นั่นคือเมื่อเบราว์เซอร์สามารถเล่นสื่อได้และคาดว่ามีการโหลดข้อมูลที่เพียงพอในการเล่นสื่อจนจบโดยไม่ต้องหยุดการเก็บเนื้อหาเพิ่มเติม

.. ``src``  String,Array: path to a video file, or array of paths for supporting different browsers
.. ``callback``  Object: callback function to be called upon 'canplaythrough' event fire, that is, when the browser can play the media, and estimates that enough data has been loaded to play the media up to its end without having to stop for further buffering of content

**ค่าที่ส่งออกมา**

- p5.MediaElement,p5.Element: ชี้ไปยังวิดีโอ p5.Element

.. p5.MediaElement,p5.Element: pointer to video p5.Element

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
