.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

input()
=======

ฟังก์ชัน. input () เรียกว่าเมื่อมีการตรวจพบอินพุตของผู้ใช้กับองค์ประกอบ เหตุการณ์อินพุตมักใช้เพื่อตรวจจับการกดแป้นพิมพ์ในอิลิเมนต์ป้อนข้อมูลหรือเปลี่ยนเป็นองค์ประกอบตัวเลื่อน สามารถใช้เพื่อแนบผู้ฟังเหตุการณ์เฉพาะบางส่วน

.. The .input() function is called when any user input is
.. detected with an element. The input event is often used
.. to detect keystrokes in a input element, or changes on a
.. slider element. This can be used to attach an element specific
.. event listener.
**รูปแบบการใช้งาน**

input ( fxn )

**พารามิเตอร์**

- ``fxn``  function: ฟังก์ชั่นที่จะใช้ในการป้อนข้อมูลของผู้ใช้

.. ``fxn``  function: function to be fired on user input.

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Open your console to see the output
	function setup() {
	  var inp = createInput('');
	  inp.input(myInputEvent);
	}
	
	function myInputEvent() {
	  console.log('you are typing: ', this.value());
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
