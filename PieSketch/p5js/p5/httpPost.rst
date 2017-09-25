.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

httpPost()
==========

Method for executing an HTTP POST request. If data type is not specified,
p5 will try to guess based on the URL, defaulting to text. This is equivalent to
calling httpDo(path, 'POST').

**รูปแบบการใช้งาน**

httpPost ( path, [datatype], [data], [callback], [errorCallback] )

**พารามิเตอร์**

- ``path``  String: name of the file or url to load

- ``datatype``  String: "json", "jsonp", "xml", or "text". If omitted, httpPost() will guess.

- ``data``  Object: param data passed sent with request

- ``callback``  function: function to be executed after httpPost() completes, data is passed in as first argument

- ``errorCallback``  function: function to be executed if there is an error, response is passed in as first argument


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Examples use jsonplaceholder.typicode.com for a Mock Data API
	
	var url = 'https://jsonplaceholder.typicode.com/posts';
	var postData = { userId: 1, title: 'p5 Clicked!', body: 'p5.js is way cool.' };
	
	function setup() {
	  createCanvas(800, 800);
	}
	
	function mousePressed() {
	 // Pick new random color values
	 var r = random(255);
	 var g = random(255);
	 var b = random(255);
	
	 httpPost(url, 'json',
	     postData,
	     function (result) {
	       strokeWeight(2);
	       stroke(r, g, b);
	       fill(r, g, b, 127);
	       ellipse(mouseX, mouseY, 200, 200);
	       text(result.body, mouseX, mouseY);
	     });
	}

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	
	 var url = 'https://invalidURL'; // A bad URL that will cause errors
	 var postData = { title: 'p5 Clicked!', body: 'p5.js is way cool.' };
	
	 function setup() {
	    createCanvas(800, 800);
	 }
	
	 function mousePressed() {
	   // Pick new random color values
	   var r = random(255);
	   var g = random(255);
	   var b = random(255);
	
	   httpPost(url, 'json',
	     postData,
	     function (result) {
	       // ... won't be called
	     },
	     function (error) {
	       strokeWeight(2);
	       stroke(r, g, b);
	       fill(r, g, b, 127);
	       text(error.toString(), mouseX, mouseY);
	   });
	 }
	

	</script>

	<br><br>

.. toctree::

