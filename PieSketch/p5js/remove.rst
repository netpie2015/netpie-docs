.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

remove()
========

ลบภาพร่าง p5 ทั้งหมด การดำเนินการนี้จะลบผ้าใบและองค์ประกอบใด ๆ ที่สร้างขึ้นโดย p5.js นอกจากนี้ยังจะหยุดการวนรอบการวาดและเลิกใช้คุณสมบัติหรือเมธอดจากขอบเขตทั่วโลกของหน้าต่าง จะออกจากตัวแปร p5 ในกรณีที่คุณต้องการสร้างร่าง p5 ใหม่ หากต้องการคุณสามารถตั้งค่า p5 = null เพื่อลบข้อมูล แม้ว่าฟังก์ชันและตัวแปรและอ็อบเจ็กต์ทั้งหมดที่สร้างขึ้นโดยไลบรารี p5 จะมีการลบตัวแปรระดับโลกอื่น ๆ ที่สร้างโดยโค้ดของคุณจะยังคงอยู่

.. Removes the entire p5 sketch. This will remove the canvas and any elements created by p5.js. It will also stop the draw loop and unbind any properties or methods from the window global scope. It will leave a variable p5 in case you wanted to create a new p5 sketch. If you like, you can set p5 = null to erase it. While all functions and variables and objects created by the p5 library will be removed, any other global variables created by your code will remain.

**รูปแบบการใช้งาน**

remove()

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function draw() {
        ellipse(50, 50, 10, 10);
    }

    function mousePressed() {
        remove(); // remove whole sketch on mouse press
    }
	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
