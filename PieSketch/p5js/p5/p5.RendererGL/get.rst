.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

get()
=====

ส่งค่าอาร์เรย์ของค่า [R, G, B, A] สำหรับพิกเซลใด ๆ หรือคว้าส่วนใดส่วนหนึ่งของรูปภาพ หากไม่มีพารามิเตอร์ระบุไว้รูปภาพทั้งหมดจะถูกส่งคืน ใช้พารามิเตอร์ x และ y เพื่อรับค่าหนึ่งพิกเซล รับส่วนของหน้าต่างการแสดงผลโดยการระบุพารามิเตอร์ w และ h เพิ่มเติม เมื่อได้รับรูปภาพพารามิเตอร์ x และ y กำหนดพิกัดสำหรับมุมซ้ายบนของภาพโดยไม่คำนึงถึง imageMode () ในปัจจุบัน 
หากพิกเซลที่ขออยู่นอกกรอบภาพจะส่งกลับ [0,0,0,255] 
การรับสีของพิกเซลเพียงจุดเดียวด้วย get (x, y) เป็นเรื่องง่าย แต่ไม่เร็วเท่าการคว้าข้อมูลโดยตรงจากพิกเซล [] คำสั่งที่เทียบเท่าเพื่อให้ได้ (x, y) ใช้พิกเซล [] ที่มีความหนาแน่นของพิกเซล d

.. Returns an array of [R,G,B,A] values for any pixel or grabs a section of
.. an image. If no parameters are specified, the entire image is returned.
.. Use the x and y parameters to get the value of one pixel. Get a section of
.. the display window by specifying additional w and h parameters. When
.. getting an image, the x and y parameters define the coordinates for the
.. upper-left corner of the image, regardless of the current imageMode().
.. 
.. If the pixel requested is outside of the image window, [0,0,0,255] is
.. returned.
.. 
.. Getting the color of a single pixel with get(x, y) is easy, but not as fast
.. as grabbing the data directly from pixels[]. The equivalent statement to
.. get(x, y) is using pixels[] with pixel density d

**รูปแบบการใช้งาน**

get ( [x], [y], [w], [h] )

**พารามิเตอร์**

- ``x``  Number: พิกัด x ของพิกเซล

- ``y``  Number: y พิกัดของพิกเซล

- ``w``  Number: ความกว้าง

- ``h``  Number: ความสูง

.. ``x``  Number: x-coordinate of the pixel
.. ``y``  Number: y-coordinate of the pixel
.. ``w``  Number: width
.. ``h``  Number: height

**ค่าที่ส่งออกมา**

- Array,Color,p5.Image: สีของพิกเซลที่ x, y ในรูปแบบอาร์เรย์ [R, G, B, A] หรือ p5.Image

.. Array,Color,p5.Image: color of pixel at x,y in array format [R, G, B, A] or p5.Image

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
