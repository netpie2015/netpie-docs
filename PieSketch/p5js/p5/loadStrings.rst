.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

loadStrings()
=============

อ่านเนื้อหาของไฟล์และสร้างอาร์เรย์สตริงของแต่ละบรรทัด ถ้าชื่อของไฟล์ถูกใช้เป็นพารามิเตอร์เช่นในตัวอย่างข้างต้นไฟล์ต้องอยู่ในไดเร็กทอรี / โฟลเดอร์สเก็ตช์ 
หรือไฟล์อาจถูกโหลดจากที่ใดก็ได้บนเครื่องคอมพิวเตอร์โดยใช้เส้นทางสัมบูรณ์ (สิ่งที่เริ่มต้นด้วย / on Unix and Linux หรืออักษรชื่อไดรฟ์ใน Windows) หรือพารามิเตอร์ชื่อไฟล์อาจเป็น URL สำหรับไฟล์ที่พบใน เครือข่าย 
วิธีนี้ไม่ตรงกันซึ่งหมายความว่าอาจไม่เสร็จสิ้นก่อนที่จะดำเนินการบรรทัดถัดไปในร่างของคุณ

.. Reads the contents of a file and creates a String array of its individual
.. lines. If the name of the file is used as the parameter, as in the above
.. example, the file must be located in the sketch directory/folder.
.. 
.. Alternatively, the file maybe be loaded from anywhere on the local
.. computer using an absolute path (something that starts with / on Unix and
.. Linux, or a drive letter on Windows), or the filename parameter can be a
.. URL for a file found on a network.
.. 
.. This method is asynchronous, meaning it may not finish before the next
.. line in your sketch is executed.
**รูปแบบการใช้งาน**

loadStrings ( filename, [callback], [errorCallback] )

**พารามิเตอร์**

- ``filename``  String: ชื่อไฟล์หรือ URL ที่จะโหลด

- ``callback``  function: ฟังก์ชันที่จะดำเนินการหลังจาก loadStrings () เสร็จสิ้นอาร์เรย์จะถูกส่งผ่านเป็นอาร์กิวเมนต์แรก

- ``errorCallback``  function: ฟังก์ชันที่จะดำเนินการถ้ามีข้อผิดพลาดการตอบสนองจะถูกส่งผ่านเป็นอาร์กิวเมนต์แรก

.. ``filename``  String: name of the file or url to load
.. ``callback``  function: function to be executed after loadStrings()
                              completes, Array is passed in as first
                              argument
.. ``errorCallback``  function: function to be executed if
                              there is an error, response is passed
                              in as first argument

**ค่าที่ส่งออกมา**

- Array.<String>: อาร์เรย์ของสตริง

.. Array.<String>: Array of Strings

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	<p>Calling loadStrings() inside preload() guarantees to complete the
	operation before setup() and draw() are called.</p>
	
	var result;
	function preload() {
	  result = loadStrings('assets/test.txt');
	}
	function setup() {
	  background(200);
	  var ind = floor(random(result.length));
	  text(result[ind], 10, 10, 80, 80);
	}
	<p>Outside of preload(), you may supply a callback function to handle the
	object:</p>
	
	function setup() {
	  loadStrings('assets/test.txt', pickString);
	}
	
	function pickString(result) {
	  background(200);
	  var ind = floor(random(result.length));
	  text(result[ind], 10, 10, 80, 80);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
