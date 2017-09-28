.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

stroke()
========

ตั้งค่าสีที่ใช้ในการวาดเส้นและเส้นขอบรอบรูปทรง สีนี้มีการระบุในรูปแบบของสี RGB หรือ HSB ขึ้นอยู่กับ colorMode ปัจจุบัน () (พื้นที่สีเริ่มต้นคือ RGB โดยแต่ละค่าจะอยู่ในช่วงตั้งแต่ 0 ถึง 255) 
ถ้ามีอาร์กิวเมนต์สตริงเดียวให้ใช้สตริงสี RGB, RGBA และ Hex CSS และสตริงสีที่มีชื่อทั้งหมด ในกรณีนี้ไม่สนับสนุนค่าตัวเลขอัลฟาเป็นอาร์กิวเมนต์ที่สองให้ใช้รูปแบบ RGBA 
วัตถุสี p5 สามารถจัดเตรียมเพื่อกำหนดสีของจังหวะ

.. Sets the color used to draw lines and borders around shapes. This color
.. is either specified in terms of the RGB or HSB color depending on the
.. current colorMode() (the default color space is RGB, with each value in
.. the range from 0 to 255).
.. 
.. If a single string argument is provided, RGB, RGBA and Hex CSS color
.. strings and all named color strings are supported. In this case, an alpha
.. number value as a second argument is not supported, the RGBA form should be
.. used.
.. 
.. A p5 Color object can also be provided to set the stroke color.

**รูปแบบการใช้งาน**

stroke ( v1, v2, v3, [alpha] )

**พารามิเตอร์**

- ``v1``  Number: สีแดงหรือสีเทียบกับช่วงสีปัจจุบัน

- ``v2``  Number: สีเขียวหรือความอิ่มตัวของสีเทียบกับช่วงสีปัจจุบัน

- ``v3``  Number: สีฟ้าหรือความสว่างเทียบกับช่วงสีปัจจุบัน

- ``alpha``  Number: 

.. ``v1``  Number: red or hue value relative to the current color range
.. ``v2``  Number: green or saturation value relative to the current color range
.. ``v3``  Number: blue or brightness value relative to the current color range
.. ``alpha``  Number: 

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
