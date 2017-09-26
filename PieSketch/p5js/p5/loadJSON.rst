.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

loadJSON()
==========

โหลดไฟล์ JSON จากไฟล์หรือ URL และส่งคืนออบเจ็กต์หรืออาร์เรย์ วิธีนี้ไม่ตรงกันซึ่งหมายความว่าอาจไม่เสร็จสิ้นก่อนที่จะดำเนินการบรรทัดถัดไปในร่างของคุณ JSONP ได้รับการสนับสนุนผ่าน polyfill และคุณสามารถส่งผ่านเป็นอาร์กิวเมนต์ที่สองของวัตถุที่มีคำจำกัดความของการเรียกกลับ json ตามไวยากรณ์ที่ระบุไว้ ที่นี่

.. Loads a JSON file from a file or a URL, and returns an Object or Array.
.. This method is asynchronous, meaning it may not finish before the next
.. line in your sketch is executed. JSONP is supported via a polyfill and you
.. can pass in as the second argument an object with definitions of the json
.. callback following the syntax specified here.
**รูปแบบการใช้งาน**

loadJSON ( path, [jsonpOptions], [datatype], [callback], [errorCallback] )

**พารามิเตอร์**

- ``path``  String: ชื่อไฟล์หรือ URL ที่จะโหลด

- ``jsonpOptions``  Object: วัตถุตัวเลือกสำหรับการตั้งค่าที่เกี่ยวข้องกับ jsonp

- ``datatype``  String: &quot;json&quot; หรือ &quot;jsonp&quot;

- ``callback``  function: ฟังก์ชันที่จะดำเนินการหลังจาก loadJSON () เสร็จสมบูรณ์แล้วข้อมูลจะถูกส่งผ่านเป็นอาร์กิวเมนต์แรก

- ``errorCallback``  function: ฟังก์ชันที่จะดำเนินการถ้ามีข้อผิดพลาดการตอบสนองจะถูกส่งผ่านเป็นอาร์กิวเมนต์แรก

.. ``path``  String: name of the file or url to load
.. ``jsonpOptions``  Object: options object for jsonp related settings
.. ``datatype``  String: "json" or "jsonp"
.. ``callback``  function: function to be executed after
                                   loadJSON() completes, data is passed
                                   in as first argument
.. ``errorCallback``  function: function to be executed if
                                   there is an error, response is passed
                                   in as first argument

**ค่าที่ส่งออกมา**

- Object,Array: ข้อมูล JSON

.. Object,Array: JSON data

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	<p>Calling loadJSON() inside preload() guarantees to complete the
	operation before setup() and draw() are called.</p>
	
	// Examples use USGS Earthquake API:
	//   https://earthquake.usgs.gov/fdsnws/event/1/#methods
	var earthquakes;
	function preload() {
	  // Get the most recent earthquake in the database
	  var url = 'https://earthquake.usgs.gov/fdsnws/event/1/query?' +
	    'format=geojson&limit=1&orderby=time';
	  earthquakes = loadJSON(url);
	}
	
	function setup() {
	  noLoop();
	}
	
	function draw() {
	  background(200);
	  // Get the magnitude and name of the earthquake out of the loaded JSON
	  var earthquakeMag = earthquakes.features[0].properties.mag;
	  var earthquakeName = earthquakes.features[0].properties.place;
	  ellipse(width/2, height/2, earthquakeMag * 10, earthquakeMag * 10);
	  textAlign(CENTER);
	  text(earthquakeName, 0, height - 30, width, 30);
	}
	
	<p>Outside of preload(), you may supply a callback function to handle the
	object:</p>
	function setup() {
	  noLoop();
	  var url = 'https://earthquake.usgs.gov/fdsnws/event/1/query?' +
	    'format=geojson&limit=1&orderby=time';
	  loadJSON(url, drawEarthquake);
	}
	
	function draw() {
	  background(200);
	}
	
	function drawEarthquake(earthquakes) {
	  // Get the magnitude and name of the earthquake out of the loaded JSON
	  var earthquakeMag = earthquakes.features[0].properties.mag;
	  var earthquakeName = earthquakes.features[0].properties.place;
	  ellipse(width/2, height/2, earthquakeMag * 10, earthquakeMag * 10);
	  textAlign(CENTER);
	  text(earthquakeName, 0, height - 30, width, 30);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
