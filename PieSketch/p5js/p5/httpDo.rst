.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

httpDo()
========

Method for executing an HTTP request. If data type is not specified,
p5 will try to guess based on the URL, defaulting to text.

For more advanced use, you may also pass in the path as the first argument
and a object as the second argument, the signature follows the one specified
in the Fetch API specification.

**รูปแบบการใช้งาน**

httpDo ( path, [method], [datatype], [data], [callback], [errorCallback] )

**พารามิเตอร์**

- ``path``  String: name of the file or url to load

- ``method``  String: either "GET", "POST", or "PUT", defaults to "GET"

- ``datatype``  String: "json", "jsonp", "xml", or "text"

- ``data``  Object: param data passed sent with request

- ``callback``  function: function to be executed after httpGet() completes, data is passed in as first argument

- ``errorCallback``  function: function to be executed if there is an error, response is passed in as first argument


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Examples use USGS Earthquake API:
	// https://earthquake.usgs.gov/fdsnws/event/1/#methods
	
	// displays an animation of all USGS earthquakes
	var earthquakes;
	var eqFeatureIndex = 0;
	
	function preload() {
	   var url = 'https://earthquake.usgs.gov/fdsnws/event/1/query?format=geojson';
	   httpDo(url,
	     {
	       method: 'GET',
	       // Other Request options, like special headers for apis
	       headers: { authorization: 'Bearer secretKey' }
	     },
	     function(res) {
	       earthquakes = res;
	     });
	}
	
	function draw() {
	   // wait until the data is loaded
	   if (!earthquakes || !earthquakes.features[eqFeatureIndex]) {
	     return;
	   }
	   clear();
	
	   var feature = earthquakes.features[eqFeatureIndex];
	   var mag = feature.properties.mag;
	   var rad = mag / 11 * ((width + height) / 2);
	   fill(255, 0, 0, 100);
	   ellipse(
	     width / 2 + random(-2, 2),
	     height / 2 + random(-2, 2),
	     rad, rad
	   );
	
	   if (eqFeatureIndex >= earthquakes.features.length) {
	     eqFeatureIndex = 0;
	   } else {
	     eqFeatureIndex += 1;
	   }
	}

	</script>

	<br><br>

.. toctree::

