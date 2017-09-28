.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

loadModel()
===========

โหลดโมเดล 3 มิติจากไฟล์ OBJ 
หนึ่งในข้อ จำกัด ของรูปแบบ OBJ คือไม่ได้มีความรู้สึกในตัวของเครื่องชั่ง ซึ่งหมายความว่าโมเดลที่ส่งออกจากโปรแกรมต่างๆอาจมีขนาดแตกต่างกันมาก หากโมเดลของคุณไม่แสดงให้ลองเรียก loadModel () โดยตั้งค่าพารามิเตอร์ normalalized เป็น true นี้จะปรับขนาดรูปแบบที่เหมาะสมกับ p5 นอกจากนี้คุณยังสามารถทำการเปลี่ยนแปลงเพิ่มเติมเกี่ยวกับขนาดที่ใหญ่ที่สุดของโมเดลด้วยฟังก์ชัน scale () ได้อีกด้วย

.. Load a 3d model from an OBJ file.
.. 
.. One of the limitations of the OBJ format is that it doesn't have a built-in
.. sense of scale. This means that models exported from different programs might
.. be very different sizes. If your model isn't displaying, try calling
.. loadModel() with the normalized parameter set to true. This will resize the
.. model to a scale appropriate for p5. You can also make additional changes to
.. the final size of your model with the scale() function.

**รูปแบบการใช้งาน**

loadModel ( path, normalize, [successCallback], [failureCallback] )

**พารามิเตอร์**

- ``path``  String: เส้นทางของโมเดลที่จะโหลด

- ``normalize``  Boolean: ถ้าเป็นจริงให้ปรับขนาดให้เป็นแบบมาตรฐานเมื่อโหลด

- ``successCallback``  function: ฟังก์ชันที่จะเรียกเมื่อมีการโหลดโมเดล จะต้องผ่านวัตถุแบบจำลอง 3 มิติ

- ``failureCallback``  function: ที่เรียกว่ามีข้อผิดพลาดของเหตุการณ์ถ้ารูปภาพไม่สามารถโหลดได้

.. ``path``  String: Path of the model to be loaded
.. ``normalize``  Boolean: If true, scale the model to a standardized size when loading
.. ``successCallback``  function: Function to be called once the model is loaded. Will be passed the 3D model object.
.. ``failureCallback``  function: called with event error if the image fails to load.

**ค่าที่ส่งออกมา**

- p5.Geometry: วัตถุ p5.Geometry

.. p5.Geometry: the p5.Geometry object

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
