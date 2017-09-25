.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

createVideo()
=============

Creates an HTML5 &lt;video&gt; element in the DOM for simple playback
of audio/video. Shown by default, can be hidden with .hide()
and drawn into canvas using video(). Appends to the container
node if one is specified, otherwise appends to body. The first parameter
can be either a single string path to a video file, or an array of string
paths to different formats of the same video. This is useful for ensuring
that your video can play across different browsers, as each supports
different formats. See this
page for further information about supported formats.

**รูปแบบการใช้งาน**

createVideo ( src, [callback] )

**พารามิเตอร์**

- ``src``  String,Array: path to a video file, or array of paths for supporting different browsers

- ``callback``  Object: callback function to be called upon 'canplaythrough' event fire, that is, when the browser can play the media, and estimates that enough data has been loaded to play the media up to its end without having to stop for further buffering of content


**ค่าที่ส่งออกมา**

- p5.MediaElement,p5.Element: pointer to video p5.Element


.. toctree::

