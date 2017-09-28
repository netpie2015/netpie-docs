.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

colorMode()
===========

colorMode () เปลี่ยนวิธี p5.js ตีความข้อมูลสี พารามิเตอร์สำหรับ fill (), stroke (), background () และ color () จะถูกกำหนดโดยค่าระหว่าง 0 ถึง 255 โดยใช้รูปแบบสี RGB นี้เทียบเท่ากับการตั้งค่า colorMode (RGB, 255) การตั้งค่า colorMode (HSB) ช่วยให้คุณใช้ระบบ HSB แทน โดยค่าเริ่มต้นนี่คือ colorMode (HSB, 360, 100, 100, 1) คุณยังสามารถใช้ HSL 
หมายเหตุ: ออบเจกต์สีที่มีอยู่จะจดจำโหมดที่สร้างขึ้นเพื่อให้คุณสามารถเปลี่ยนโหมดได้ตามต้องการโดยไม่ส่งผลกระทบต่อรูปลักษณ์

.. colorMode() changes the way p5.js interprets color data. By default, the
.. parameters for fill(), stroke(), background(), and color() are defined by
.. values between 0 and 255 using the RGB color model. This is equivalent to
.. setting colorMode(RGB, 255). Setting colorMode(HSB) lets you use the HSB
.. system instead. By default, this is colorMode(HSB, 360, 100, 100, 1). You
.. can also use HSL.
.. 
.. Note: existing color objects remember the mode that they were created in,
.. so you can change modes as you like without affecting their appearance.

**รูปแบบการใช้งาน**

colorMode ( mode, [max] )

**พารามิเตอร์**

- ``mode``  Constant: RGB, HSB หรือ HSL ซึ่งสอดคล้องกับสีแดง / เขียว / น้ำเงินและสี / ความอิ่มตัว / ความสว่าง (หรือความสว่าง)

- ``max``  Number: ช่วงสำหรับค่าทั้งหมด

.. ``mode``  Constant: either RGB, HSB or HSL, corresponding to Red/Green/Blue and Hue/Saturation/Brightness (or Lightness)
.. ``max``  Number: range for all values

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
