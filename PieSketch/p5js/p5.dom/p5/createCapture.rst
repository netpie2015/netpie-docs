.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

createCapture()
===============

Creates a new &lt;video&gt; element that contains the audio/video feed
from a webcam. This can be drawn onto the canvas using video().
More specific properties of the feed can be passing in a Constraints object.
See the W3C spec for possible properties. Note that not all of these are supported
by all browsers.

Security note: A new browser security specification requires that getUserMedia,
which is behind createCapture(), only works when you're running the code locally,
or on HTTPS. Learn more here
and here.

**รูปแบบการใช้งาน**

createCapture ( type, callback )

**พารามิเตอร์**

- ``type``  String,Constant,Object: type of capture, either VIDEO or AUDIO if none specified, default both, or a Constraints object

- ``callback``  function: function to be called once stream has loaded


**ค่าที่ส่งออกมา**

- Object,p5.Element: capture video p5.Element


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

.. toctree::

