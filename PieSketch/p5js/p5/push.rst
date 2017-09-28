.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

push()
======

ฟังก์ชัน push () จะบันทึกการตั้งค่ารูปแบบการวาดภาพปัจจุบันและการแปลงในขณะที่ pop () คืนค่าการตั้งค่าเหล่านี้ โปรดทราบว่าฟังก์ชันเหล่านี้ใช้กันอยู่เสมอ พวกเขาช่วยให้คุณสามารถเปลี่ยนรูปแบบและการตั้งค่าการแปลงและภายหลังกลับไปสิ่งที่คุณมี เมื่อสถานะใหม่เริ่มต้นด้วย push () จะสร้างสไตล์และเปลี่ยนข้อมูลปัจจุบัน สามารถฝังฟังก์ชัน push () และ pop () เพื่อให้สามารถควบคุมได้มากขึ้น (ดูตัวอย่างที่สองสำหรับการสาธิต) 
push () เก็บข้อมูลที่เกี่ยวข้องกับสถานะปัจจุบันของการแปลงและการตั้งค่าสไตล์ที่ควบคุมโดยฟังก์ชันต่อไปนี้: fill (), stroke (), tint (), strokeWeight (), strokeCap ​​(), strokeJoin (), imageMode (), rectMode ( ), ellipseMode (), colorMode (), textAlign (), textFont (), textMode (), textSize (), textLeading ()

.. The push() function saves the current drawing style settings and
.. transformations, while pop() restores these settings. Note that these
.. functions are always used together. They allow you to change the style
.. and transformation settings and later return to what you had. When a new
.. state is started with push(), it builds on the current style and transform
.. information. The push() and pop() functions can be embedded to provide
.. more control. (See the second example for a demonstration.)
.. 
.. push() stores information related to the current transformation state
.. and style settings controlled by the following functions: fill(),
.. stroke(), tint(), strokeWeight(), strokeCap(), strokeJoin(),
.. imageMode(), rectMode(), ellipseMode(), colorMode(), textAlign(),
.. textFont(), textMode(), textSize(), textLeading().

**รูปแบบการใช้งาน**

push ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	ellipse(0, 50, 33, 33);  // Left circle
	
	push();  // Start a new drawing state
	strokeWeight(10);
	fill(204, 153, 0);
	translate(50, 0);
	ellipse(0, 50, 33, 33);  // Middle circle
	pop();  // Restore original state
	
	ellipse(100, 50, 33, 33);  // Right circle

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	ellipse(0, 50, 33, 33);  // Left circle
	
	push();  // Start a new drawing state
	strokeWeight(10);
	fill(204, 153, 0);
	ellipse(33, 50, 33, 33);  // Left-middle circle
	
	push();  // Start another new drawing state
	stroke(0, 102, 153);
	ellipse(66, 50, 33, 33);  // Right-middle circle
	pop();  // Restore previous state
	
	pop();  // Restore original state
	
	ellipse(100, 50, 33, 33);  // Right circle

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
