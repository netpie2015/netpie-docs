.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

draw()
======

เรียกฟังก์ชันโดยตรง () หลังจากตั้งค่า () ฟังก์ชัน draw () จะดำเนินการบรรทัดของรหัสที่อยู่ภายในบล็อกจนกว่าจะมีการหยุดโปรแกรมหรือเรียก noLoop () หมายเหตุถ้าเรียกว่า noLoop () ในการตั้งค่า (), draw () จะยังคงทำงานได้เพียงครั้งเดียวก่อนที่จะหยุด วาด () เรียกโดยอัตโนมัติและไม่ควรเรียกอย่างชัดแจ้ง

ควรควบคุมด้วย noLoop (), redraw () และ loop () หลังจาก noLoop () หยุดโค้ดใน draw () จากการดำเนินการการวาดใหม่ () จะทำให้โค้ดภายใน draw () ใช้ครั้งเดียวและ loop () จะทำให้โค้ดภายใน draw () ทำงานต่อไปอย่างต่อเนื่อง

จำนวนครั้งที่วาด () ในแต่ละวินาทีอาจถูกควบคุมด้วยฟังก์ชัน frameRate ()

มีเพียงหนึ่งวาด () สำหรับแต่ละร่างและวาด () ต้องมีอยู่ถ้าคุณต้องการให้รหัสทำงานอย่างต่อเนื่องหรือเพื่อประมวลผลเหตุการณ์เช่น mousePressed () บางครั้งคุณอาจมีสายที่ว่างเปล่าในการวาด () ในโปรแกรมดังที่แสดงไว้ในตัวอย่างข้างต้น

เป็นสิ่งสำคัญที่จะต้องทราบว่าระบบพิกัดการวาดภาพจะถูกรีเซ็ตที่จุดเริ่มต้นของการวาดแต่ละครั้ง หากมีการแปลงใด ๆ เกิดขึ้นภายในวาด () (เช่น scale, rotate, translate, effect จะถูกยกเลิกเมื่อเริ่มวาดภาพ) ดังนั้นการแปลงจะไม่เกิดขึ้นตลอดเวลาในทางกลับกันการจัดแต่งทรงผม (เช่น fill , จังหวะ ฯลฯ ) จะยังคงมีผล

.. Called directly after setup(), the draw() function continuously executes the lines of code contained inside its block until the program is stopped or noLoop() is called. Note if noLoop() is called in setup(), draw() will still be executed once before stopping. draw() is called automatically and should never be called explicitly. 
.. It should always be controlled with noLoop(), redraw() and loop(). After noLoop() stops the code in draw() from executing, redraw() causes the code inside draw() to execute once, and loop() will cause the code inside draw() to resume executing continuously.
.. The number of times draw() executes in each second may be controlled with the frameRate() function. 
.. There can only be one draw() function for each sketch, and draw() must exist if you want the code to run continuously, or to process events such as mousePressed(). Sometimes, you might have an empty call to draw() in your program, as shown in the above example.
.. It is important to note that the drawing coordinate system will be reset at the beginning of each draw() call. If any transformations are performed within draw() (ex: scale, rotate, translate, their effects will be undone at the beginning of draw(), so transformations will not accumulate over time. On the other hand, styling applied (ex: fill, stroke, etc) will remain in effect.

**รูปแบบการใช้งาน**

draw()

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var yPos = 0;
    function setup() {  // setup() runs once
    frameRate(30);
    }
    function draw() {  // draw() loops forever, until stopped
    background(204);
    yPos = yPos - 1;
    if (yPos < 0) {
        yPos = height;
    }
    line(0, yPos, width, yPos);
    }
	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
