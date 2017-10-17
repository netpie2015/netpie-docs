.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

resize()
========

ปรับขนาดภาพใหม่เป็นความกว้างและความสูง หากต้องการปรับสัดส่วนภาพให้เหมาะสมให้ใช้ 0 เป็นค่าสำหรับพารามิเตอร์กว้างหรือสูง ตัวอย่างเช่นเพื่อให้ความกว้างของภาพ 150 พิกเซลและเปลี่ยนความสูงโดยใช้สัดส่วนเดียวกันให้ใช้การปรับขนาด (150, 0)

.. Resize the image to a new width and height. To make the image scale
.. proportionally, use 0 as the value for the wide or high parameter.
.. For instance, to make the width of an image 150 pixels, and change
.. the height using the same proportion, use resize(150, 0).

**รูปแบบการใช้งาน**

resize ( width, height )

**พารามิเตอร์**

- ``width``  Number: ความกว้างของภาพที่ปรับขนาดได้

- ``height``  Number: ความสูงของภาพที่ปรับขนาด

.. ``width``  Number: the resized image width
.. ``height``  Number: the resized image height

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var img;
	
	function setup() {
	  img = loadImage("assets/rockies.jpg");
	}
	function draw() {
	  image(img, 0, 0);
	}
	
	function mousePressed() {
	  img.resize(50, 100);
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
