.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

tint()
======

ตั้งค่าการเติมสำหรับแสดงภาพ ภาพสามารถย้อมสีให้เป็นสีที่กำหนดหรือทำให้มีความโปร่งใสโดยรวมค่า alpha

หากต้องการใช้ความโปร่งใสกับภาพโดยไม่มีผลต่อสีให้ใช้สีขาวเป็นสีของสีและระบุค่า alpha ตัวอย่างเช่นสี (255, 128) จะทำให้ภาพโปร่งใส 50% (สมมติว่าช่วง alpha เริ่มต้นเป็น 0-255 ซึ่งสามารถเปลี่ยนได้ด้วย colorMode ())

ค่าสำหรับพารามิเตอร์สีเทาต้องน้อยกว่าหรือเท่ากับค่าสูงสุดปัจจุบันที่ระบุโดย colorMode () ค่าสูงสุดเริ่มต้นคือ 255

.. Sets the fill value for displaying images. Images can be tinted to specified colors or made transparent by including an alpha value.
.. To apply transparency to an image without affecting its color, use white as the tint color and specify an alpha value. For instance, tint(255, 128) will make an image 50% transparent (assuming the default alpha range of 0-255, which can be changed with colorMode()).
.. The value for the gray parameter must be less than or equal to the current maximum value as specified by colorMode(). The default maximum value is 255.

**รูปแบบการใช้งาน**

tint(v1,v2,v3,[alpha])

tint(value,[alpha])

tint(values)

tint(color,[alpha])

**พารามิเตอร์**

- ``v1``  ตัวเลข: ค่าสีแดงหรือสีที่สัมพันธ์กับช่วงสีปัจจุบัน

- ``v2``  ตัวเลข: สีเขียวหรือความอิ่มตัวของสีเทียบกับช่วงสีปัจจุบัน

- ``v3``  ตัวเลข: สีฟ้าหรือความสว่างเทียบกับช่วงสีปัจจุบัน

- ``alpha``  ตัวเลข

- ``value``  สตริง: สตริงสี

- ``values``  ตัวเลข[]: อาร์เรย์ที่ประกอบด้วยองค์ประกอบสีแดงสีเขียวฟ้าและสีอัลฟา

- ``color``  p5.Color: สีของสี

.. ``v1``  Number: red or hue value relative to the current color range
.. ``v2``  Number: green or saturation value relative to the current color range
.. ``v3``  Number: blue or brightness value relative to the current color range
.. ``alpha``  Number
.. ``value``  String: a color string
.. ``values``  Number[]: an array containing the red,green,blue & and alpha components of the color
.. ``color``  p5.Color: the tint color

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
