.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

arc()
=====


วาดส่วนโค้งบนหน้าจอ หากมีการส่งผ่านค่าพารามิเตอร์ไม่ครบ คือส่งเข้ามาเพียง a, b, c, d, start และ stop จะเป็นการวาดส่วนโค้งวงกลมแบบเปิด แต่หากมีการส่งพารามิเตอร์ mode ส่วนโค้งที่วาดสามารถเป็นได้ทั้งแบบเปิด (OPEN) หรือเป็นคอร์ด (CHORD) หรือเป็นรูปพาย (PIE) แล้วแต่จะระบุ จุดศูนย์กลางของส่วนโค้งสามารถเปลี่ยนค่าได้ โดยใช้ฟังก์ชัน ellipseMode()

ท้งนี้การสั่งวาดวงกลมแบบเต็มวง (คือลากจาก 0 ถึง TWO_PI) จะไม่ปรากฏเส้นโค้งใดๆ เนื่องจาก 0 โค้งใดๆและ TWO_PI เป็นตำแหน่งจุดเดียวกันในวงกลม วิธีที่ดีที่สุดในการจัดการคือ การใช้ฟังก์ชัน ellipse() แทนที่จะสร้างรูปวงกลมหรือวงรีที่ปิด และใช้ฟังก์ชัน arc() เพื่อวาดส่วนของวงกลมหรือวงรี

**รูปแบบการใช้งาน**

arc (*a,b,c,d,start,stop,[mode]* )

**พารามิเตอร์**


.. raw:: html

	<script type="text/p5" data-autoplay data-height="220">
	function setup() {
	    arc(50, 50, 80, 80, 0, PI+QUARTER_PI, OPEN);
	}
	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-height="220">
	function setup() {
	    arc(50, 50, 80, 80, 0, PI+QUARTER_PI, CHORD);
	}
	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-height="220">
	function setup() {
	    arc(50, 50, 80, 80, 0, PI+QUARTER_PI, PIE);
	}
	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-height="280">
	function setup() {
	    arc(50, 55, 50, 50, 0, HALF_PI);
	    noFill();
	    arc(50, 55, 60, 60, HALF_PI, PI);
	    arc(50, 55, 70, 70, PI, PI+QUARTER_PI);
	    arc(50, 55, 80, 80, PI+QUARTER_PI, TWO_PI);
	}
	</script>


.. toctree::
