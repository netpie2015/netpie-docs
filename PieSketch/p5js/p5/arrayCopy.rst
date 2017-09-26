.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

arrayCopy()
===========

คัดลอกอาร์เรย์ (หรือบางส่วนของอาร์เรย์) ไปยังอาร์เรย์อื่น อาร์เรย์ src ถูกคัดลอกไปยังอาร์เรย์ dst โดยเริ่มจากตำแหน่งที่ระบุโดย srcPosition และอยู่ในตำแหน่งที่ระบุโดย dstPosition จำนวนองค์ประกอบที่จะคัดลอกจะถูกกำหนดตามความยาว โปรดทราบว่าการคัดลอกค่าจะเขียนทับค่าที่มีอยู่ในอาร์เรย์ปลายทาง หากต้องการผนวกค่าแทนการเขียนทับให้ใช้ concat () 
อาร์เรย์ทั้งหมดมีอาร์กิวเมนต์เพียงสองอาร์กิวเมนต์ arrayCopy (src, dst) คัดลอกอาร์เรย์ทั้งหมดไปยังอีกที่มีขนาดเท่ากัน เทียบเท่ากับ arrayCopy (src, 0, dst, 0, src.length) 
การใช้ฟังก์ชันนี้มีประสิทธิภาพมากขึ้นในการคัดลอกข้อมูลอาร์เรย์มากกว่าการวนซ้ำผ่านลูป for () และการคัดลอกแต่ละองค์ประกอบทีละรายการ

.. Copies an array (or part of an array) to another array. The src array is
.. copied to the dst array, beginning at the position specified by
.. srcPosition and into the position specified by dstPosition. The number of
.. elements to copy is determined by length. Note that copying values
.. overwrites existing values in the destination array. To append values
.. instead of overwriting them, use concat().
.. 
.. The simplified version with only two arguments, arrayCopy(src, dst),
.. copies an entire array to another of the same size. It is equivalent to
.. arrayCopy(src, 0, dst, 0, src.length).
.. 
.. Using this function is far more efficient for copying array data than
.. iterating through a for() loop and copying each element individually.

**รูปแบบการใช้งาน**

arrayCopy ( src, srcPosition, dst, dstPosition, length )

**พารามิเตอร์**

- ``src``  Array: อาร์เรย์ของแหล่งที่มา

- ``srcPosition``  Number: ตำแหน่งเริ่มต้นในแหล่ง Array

- ``dst``  Array: อาร์เรย์ปลายทาง

- ``dstPosition``  Number: ตำแหน่งเริ่มต้นในอาร์เรย์ปลายทาง

- ``length``  Number: จำนวนอาร์เรย์ที่จะคัดลอก

.. ``src``  Array: the source Array
.. ``srcPosition``  Number: starting position in the source Array
.. ``dst``  Array: the destination Array
.. ``dstPosition``  Number: starting position in the destination Array
.. ``length``  Number: number of Array elements to be copied

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
