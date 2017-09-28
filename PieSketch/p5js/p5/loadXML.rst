.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

loadXML()
=========

อ่านเนื้อหาของไฟล์และสร้างอ็อบเจ็กต์ XML ด้วยค่าของไฟล์ ถ้าชื่อของไฟล์ถูกใช้เป็นพารามิเตอร์เช่นในตัวอย่างข้างต้นไฟล์ต้องอยู่ในไดเร็กทอรี / โฟลเดอร์สเก็ตช์ หรือไฟล์อาจถูกโหลดจากที่ใดก็ได้บนเครื่องคอมพิวเตอร์โดยใช้เส้นทางสัมบูรณ์ (สิ่งที่เริ่มต้นด้วย / on Unix and Linux หรืออักษรชื่อไดรฟ์ใน Windows) หรือพารามิเตอร์ชื่อไฟล์อาจเป็น URL สำหรับไฟล์ที่พบใน เครือข่าย วิธีนี้ไม่ตรงกันซึ่งหมายความว่าอาจไม่เสร็จสิ้นก่อนที่จะดำเนินการบรรทัดถัดไปในร่างของคุณ การเรียก loadXML () ภายใน preload () รับประกันว่าจะดำเนินการให้เสร็จสิ้นก่อนที่จะเรียกการตั้งค่า () และ draw () นอกเหนือจาก preload () คุณอาจจะจัดหาฟังก์ชัน callback เพื่อจัดการวัตถุ

.. Reads the contents of a file and creates an XML object with its values.
.. If the name of the file is used as the parameter, as in the above example,
.. the file must be located in the sketch directory/folder.
.. Alternatively, the file maybe be loaded from anywhere on the local
.. computer using an absolute path (something that starts with / on Unix and
.. Linux, or a drive letter on Windows), or the filename parameter can be a
.. URL for a file found on a network.
.. This method is asynchronous, meaning it may not finish before the next
.. line in your sketch is executed. Calling loadXML() inside preload()
.. guarantees to complete the operation before setup() and draw() are called.
.. Outside of preload(), you may supply a callback function to handle the
.. object.

**รูปแบบการใช้งาน**

loadXML ( filename, [callback], [errorCallback] )

**พารามิเตอร์**

- ``filename``  String: ชื่อไฟล์หรือ URL ที่จะโหลด

- ``callback``  function: ฟังก์ชันที่จะดำเนินการหลังจาก loadXML () เสร็จสมบูรณ์แล้ววัตถุ XML ถูกส่งผ่านเป็นอาร์กิวเมนต์แรก

- ``errorCallback``  function: ฟังก์ชันที่จะดำเนินการถ้ามีข้อผิดพลาดการตอบสนองจะถูกส่งผ่านเป็นอาร์กิวเมนต์แรก

.. ``filename``  String: name of the file or URL to load
.. ``callback``  function: function to be executed after loadXML() completes, XML object is passed in as first argument
.. ``errorCallback``  function: function to be executed if there is an error, response is passed in as first argument

**ค่าที่ส่งออกมา**

- Object: วัตถุ XML ที่มีข้อมูล

.. Object: XML object containing data

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// The following short XML file called "mammals.xml" is parsed
	// in the code below.
	//
	// <?xml version="1.0"?>
	// &lt;mammals&gt;
	//   &lt;animal id="0" species="Capra hircus">Goat&lt;/animal&gt;
	//   &lt;animal id="1" species="Panthera pardus">Leopard&lt;/animal&gt;
	//   &lt;animal id="2" species="Equus zebra">Zebra&lt;/animal&gt;
	// &lt;/mammals&gt;
	
	var xml;
	
	function preload() {
	  xml = loadXML("assets/mammals.xml");
	}
	
	function setup() {
	  var children = xml.getChildren("animal");
	
	  for (var i = 0; i < children.length; i++) {
	    var id = children[i].getNum("id");
	    var coloring = children[i].getString("species");
	    var name = children[i].getContent();
	    print(id + ", " + coloring + ", " + name);
	  }
	}
	
	// Sketch prints:
	// 0, Capra hircus, Goat
	// 1, Panthera pardus, Leopard
	// 2, Equus zebra, Zebra

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
