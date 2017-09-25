.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

saveFrames()
============

Capture a sequence of frames that can be used to create a movie.
 Accepts a callback. For example, you may wish to send the frames
 to a server where they can be stored or converted into a movie.
 If no callback is provided, the browser will pop up save dialogues in an
 attempt to download all of the images that have just been created. With the
 callback provided the image data isn't saved by default but instead passed
 as an argument to the callback function as an array of objects, with the
 size of array equal to the total number of frames.

**รูปแบบการใช้งาน**

saveFrames ( filename, extension, duration, framerate, [callback] )

**พารามิเตอร์**

- ``filename``  String: 

- ``extension``  String: 'jpg' or 'png'

- ``duration``  Number: Duration in seconds to save the frames for.

- ``framerate``  Number: Framerate to save the frames in.

- ``callback``  function: A callback function that will be executed to handle the image data. This function should accept an array as argument. The array will contain the specified number of frames of objects. Each object has three properties: imageData - an image/octet-stream, filename and extension.


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	 function draw() {
	   background(mouseX);
	 }
	
	 function mousePressed() {
	   saveFrames("out", "png", 1, 25, function(data){
	     print(data);
	   });
	 }
	 

	</script>

	<br><br>

.. toctree::

