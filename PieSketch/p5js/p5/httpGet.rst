.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

httpGet()
=========

วิธีการดำเนินการคำขอ HTTP GET หากไม่มีการระบุชนิดข้อมูล p5 จะพยายามคาดเดาตาม URL ซึ่งเป็นค่าเริ่มต้นเป็นข้อความ นี่เทียบเท่ากับการเรียก httpDo(path, 'GET')

.. Method for executing an HTTP GET request. If data type is not specified,
.. p5 will try to guess based on the URL, defaulting to text. This is equivalent to
.. calling httpDo(path, 'GET').

**รูปแบบการใช้งาน**

httpGet ( path, [datatype], [data], [callback], [errorCallback] )

**พารามิเตอร์**

- ``path``  String: ชื่อไฟล์หรือ URL ที่จะโหลด

- ``datatype``  String: &quot;json&quot;, &quot;jsonp&quot;, &quot;xml&quot; หรือ &quot;ข้อความ&quot;

- ``data``  Object: ข้อมูล param ที่ส่งมาพร้อมกับคำขอ

- ``callback``  function: ฟังก์ชันที่จะดำเนินการหลังจาก httpget () เสร็จสมบูรณ์แล้วข้อมูลจะถูกส่งผ่านเป็นอาร์กิวเมนต์แรก

- ``errorCallback``  function: ฟังก์ชันที่จะดำเนินการถ้ามีข้อผิดพลาดการตอบสนองจะถูกส่งผ่านเป็นอาร์กิวเมนต์แรก

.. ``path``  String: name of the file or url to load
.. ``datatype``  String: "json", "jsonp", "xml", or "text"
.. ``data``  Object: param data passed sent with request
.. ``callback``  function: function to be executed after httpGet() completes, data is passed in as first argument
.. ``errorCallback``  function: function to be executed if there is an error, response is passed in as first argument

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	 // Examples use USGS Earthquake API:
	 //   https://earthquake.usgs.gov/fdsnws/event/1/#methods
	 var earthquakes;
	 function preload() {
	   // Get the most recent earthquake in the database
	   var url = 'https://earthquake.usgs.gov/fdsnws/event/1/query?' +
	     'format=geojson&limit=1&orderby=time';
	   httpGet(url, "jsonp", false, function(response) {
	     // when the HTTP request completes, populate the variable that holds the
	     // earthquake data used in the visualization.
	     earthquakes = response;
	   });
	 }
	
	 function draw() {
	   if (!earthquakes) {
	     // Wait until the earthquake data has loaded before drawing.
	     return
	   }
	   background(200);
	   // Get the magnitude and name of the earthquake out of the loaded JSON
	   var earthquakeMag = earthquakes.features[0].properties.mag;
	   var earthquakeName = earthquakes.features[0].properties.place;
	   ellipse(width/2, height/2, earthquakeMag * 10, earthquakeMag * 10);
	   textAlign(CENTER);
	   text(earthquakeName, 0, height - 30, width, 30);
	   noLoop();
	 }

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
