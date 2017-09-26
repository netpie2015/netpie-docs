.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

saveFrames()
============

จับภาพลำดับเฟรมที่สามารถใช้ในการสร้างภาพยนตร์ ยอมรับการโทรกลับ ตัวอย่างเช่นคุณอาจต้องการส่งเฟรมไปยังเซิร์ฟเวอร์ซึ่งสามารถจัดเก็บหรือแปลงเป็นภาพเคลื่อนไหวได้ หากไม่มีการเรียกกลับมาเบราว์เซอร์จะปรากฏขึ้นเพื่อบันทึกการสนทนาด้วยความพยายามที่จะดาวน์โหลดภาพทั้งหมดที่เพิ่งสร้างขึ้น ด้วยการเรียกกลับให้ข้อมูลภาพไม่ได้รับการบันทึกไว้โดยค่าเริ่มต้น แต่แทนที่จะส่งผ่านเป็นอาร์กิวเมนต์ไปยังฟังก์ชัน callback เป็นอาร์เรย์ของอ็อบเจ็กต์โดยมีขนาดของอาร์เรย์เท่ากับจำนวนรวมของเฟรม

.. Capture a sequence of frames that can be used to create a movie.
..  Accepts a callback. For example, you may wish to send the frames
..  to a server where they can be stored or converted into a movie.
..  If no callback is provided, the browser will pop up save dialogues in an
..  attempt to download all of the images that have just been created. With the
..  callback provided the image data isn't saved by default but instead passed
..  as an argument to the callback function as an array of objects, with the
..  size of array equal to the total number of frames.
**รูปแบบการใช้งาน**

saveFrames ( filename, extension, duration, framerate, [callback] )

**พารามิเตอร์**

- ``filename``  String: 

- ``extension``  String: &#39;jpg&#39; หรือ &#39;png&#39;

- ``duration``  Number: ระยะเวลาเป็นวินาทีเพื่อบันทึกเฟรมสำหรับ

- ``framerate``  Number: Framerate เพื่อบันทึกเฟรมมา

- ``callback``  function: ฟังก์ชันเรียกกลับที่จะดำเนินการเพื่อจัดการกับข้อมูลภาพ ฟังก์ชันนี้ควรยอมรับอาร์เรย์เป็นอาร์กิวเมนต์ อาร์เรย์จะมีจำนวนเฟรมของออบเจ็กต์ที่ระบุไว้ แต่ละอ็อบเจ็กต์มีคุณสมบัติสามอย่าง: imageData - image / octet-stream, filename และ extension

.. ``filename``  String: 
.. ``extension``  String: 'jpg' or 'png'
.. ``duration``  Number: Duration in seconds to save the frames for.
.. ``framerate``  Number: Framerate to save the frames in.
.. ``callback``  function: A callback function that will be executed
                                  to handle the image data. This function
                                  should accept an array as argument. The
                                  array will contain the specified number of
                                  frames of objects. Each object has three
                                  properties: imageData - an
                                  image/octet-stream, filename and extension.

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	 function draw() {
	   background(mouseX);
	 }
	
	 function mousePressed() {
	   saveFrames("out", "png", 1, 25, function(data){
	     print(data);
	   });
	 }
	 

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
