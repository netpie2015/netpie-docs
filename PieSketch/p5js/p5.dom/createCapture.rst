.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

createCapture()
===============

 สร้าง  องค์ประกอบใหม่ที่มีฟีดเสียง / วิดีโอจากเว็บแคม ซึ่งสามารถวาดลงบนผืนผ้าใบโดยใช้วิดีโอ ()  คุณสมบัติเฉพาะของฟีดอาจส่งผ่านไปได้ในออบเจกต์ Constraints ดู ข้อมูลจำเพาะของ W3C สำหรับคุณสมบัติที่เป็นไปได้ โปรดทราบว่าเบราเซอร์ทุกตัวไม่สามารถใช้งานได้ทั้งหมด  หมายเหตุด้านความปลอดภัย: ข้อกำหนดด้านความปลอดภัยของเบราเซอร์ใหม่จำเป็นต้องใช้ getUserMedia ซึ่งอยู่เบื้องหลัง createCapture () เฉพาะเมื่อคุณใช้งานโค้ดภายในเครื่องเท่านั้นหรือบน HTTPS เรียนรู้เพิ่มเติม ที่นี่ และ ที่นี่ 

.. Creates a new &lt;video&gt; element that contains the audio/video feed
.. from a webcam. This can be drawn onto the canvas using video().
.. More specific properties of the feed can be passing in a Constraints object.
.. See the
..  W3C
.. spec for possible properties. Note that not all of these are supported
.. by all browsers.
.. Security note: A new browser security specification requires that getUserMedia,
.. which is behind createCapture(), only works when you're running the code locally,
.. or on HTTPS. Learn more here
.. and here.

**รูปแบบการใช้งาน**

createCapture ( type, callback )

**พารามิเตอร์**

- ``type``  String,Constant,Object: ชนิดของการจับภาพไม่ว่าจะเป็น VIDEO หรือ AUDIO หากไม่มีการระบุค่าเริ่มต้นทั้งสองอย่างหรือวัตถุข้อ จำกัด

- ``callback``  function: ฟังก์ชันที่จะเรียกว่าเมื่อสตรีมได้โหลด

.. ``type``  String,Constant,Object: type of capture, either VIDEO or AUDIO if none specified, default both, or a Constraints object
.. ``callback``  function: function to be called once stream has loaded

**ค่าที่ส่งออกมา**

- Object,p5.Element: จับภาพวิดีโอ p5.Element

.. Object,p5.Element: capture video p5.Element

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var capture;
	
	function setup() {
	  createCanvas(480, 120);
	  capture = createCapture(VIDEO);
	}
	
	function draw() {
	  image(capture, 0, 0, width, width*capture.height/capture.width);
	  filter(INVERT);
	}
	function setup() {
	  createCanvas(480, 120);
	  var constraints = {
	    video: {
	      mandatory: {
	        minWidth: 1280,
	        minHeight: 720
	      },
	      optional: [
	        { maxFrameRate: 10 }
	      ]
	    },
	    audio: true
	  };
	  createCapture(constraints, function(stream) {
	    console.log(stream);
	  });
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
