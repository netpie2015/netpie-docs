.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

setup()
=======

ฟังก์ชั่น setup () เรียกว่าครั้งเดียวเมื่อโปรแกรมเริ่มทำงาน ใช้เพื่อกำหนดคุณสมบัติของสภาวะแวดล้อมเริ่มต้นเช่นขนาดหน้าจอและสีพื้นหลังและโหลดสื่อเช่นรูปภาพและแบบอักษรขณะที่โปรแกรมเริ่มทำงาน สามารถใช้ฟังก์ชันการตั้งค่า () สำหรับแต่ละโปรแกรมได้เพียงครั้งเดียวและไม่ควรเรียกอีกครั้งหลังจากเริ่มต้นใช้งาน

หมายเหตุ: ตัวแปรที่ประกาศภายใน setup () ไม่สามารถเข้าถึงได้ภายในฟังก์ชันอื่น ๆ รวมถึง draw ()

.. The setup() function is called once when the program starts. It's used to define initial environment properties such as screen size and background color and to load media such as images and fonts as the program starts. There can only be one setup() function for each program and it shouldn't be called again after its initial execution.
.. Note: Variables declared within setup() are not accessible within other functions, including draw().

**รูปแบบการใช้งาน**

setup()

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var a = 0;

    function setup() {
        background(0);
        noStroke();
        fill(102);
    }

    function draw() {
        rect(a++%width, 10, 2, 80);
    }
	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
