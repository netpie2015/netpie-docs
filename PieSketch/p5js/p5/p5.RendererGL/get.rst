.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

get()
=====

Returns an array of [R,G,B,A] values for any pixel or grabs a section of
an image. If no parameters are specified, the entire image is returned.
Use the x and y parameters to get the value of one pixel. Get a section of
the display window by specifying additional w and h parameters. When
getting an image, the x and y parameters define the coordinates for the
upper-left corner of the image, regardless of the current imageMode().

If the pixel requested is outside of the image window, [0,0,0,255] is
returned.

Getting the color of a single pixel with get(x, y) is easy, but not as fast
as grabbing the data directly from pixels[]. The equivalent statement to
get(x, y) is using pixels[] with pixel density d

**รูปแบบการใช้งาน**

get ( [x], [y], [w], [h] )

**พารามิเตอร์**

- ``x``  Number: x-coordinate of the pixel

- ``y``  Number: y-coordinate of the pixel

- ``w``  Number: width

- ``h``  Number: height


**ค่าที่ส่งออกมา**

- Array,Color,p5.Image: color of pixel at x,y in array format [R, G, B, A] or p5.Image


.. toctree::

