.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

center()
========

กำหนดองค์ประกอบ p5 ทั้งแนวตั้งหรือแนวนอนหรือทั้งสองแบบเทียบกับส่วนที่เป็นแม่หรือตามร่างกายหากองค์ประกอบไม่มีผู้ปกครอง ถ้าอาร์กิวเมนต์ไม่ผ่าน Element ถูกจัดแนวทั้งแนวตั้งและแนวนอน

.. Centers a p5 Element either vertically, horizontally,
.. or both, relative to its parent or according to
.. the body if the Element has no parent. If no argument is passed
.. the Element is aligned both vertically and horizontally.

**รูปแบบการใช้งาน**

center ( align )

**พารามิเตอร์**

- ``align``  String: ผ่าน &#39;แนวตั้ง&#39;, &#39;แนวนอน&#39; จัดองค์ประกอบตาม

.. ``align``  String: passing 'vertical', 'horizontal' aligns element accordingly

**ค่าที่ส่งออกมา**

- Object,p5.Element: ชี้ไปที่ p5.Element

.. Object,p5.Element: pointer to p5.Element

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var div = createDiv('').size(10,10);
	  div.style('background-color','orange');
	  div.center();
	
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
