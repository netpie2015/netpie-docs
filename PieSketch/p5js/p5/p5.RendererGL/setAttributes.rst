.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

setAttributes()
===============

ตั้งค่าแอตทริบิวต์สำหรับบริบทการเขียนแบบ WebGL นี่เป็นวิธีการปรับวิธีที่ renderer ของ WebGL ทำงานเพื่อปรับแต่งการแสดงผลและประสิทธิภาพการทำงาน นี้ควรจะใส่ในการติดตั้ง () แอตทริบิวต์ที่มีอยู่ ได้แก่ 
alpha - ระบุว่าผ้าใบมีค่าดีฟอลต์บัฟเฟอร์ alpha เป็นจริงหรือไม่ 
depth - ระบุว่าบัฟเฟอร์การวาดภาพมี buffer อย่างน้อย 16 bits หรือไม่ - default คือ true 
stencil - ระบุว่าบัฟเฟอร์รูปวาดมีบัฟเฟอร์ stencil อย่างน้อย 8 บิต 
antialias - ระบุว่าจะใช้ค่าเริ่มต้น anti-aliasing หรือไม่เป็นเท็จ 
premultipliedAlpha - ระบุว่า compositor หน้าจะถือว่าบัฟเฟอร์การวาดภาพมีสีที่มีค่าเริ่มต้นอัลฟ่าก่อนคูณเป็นเท็จ 
preserveDrawingBuffer - ถ้า true บัฟเฟอร์จะไม่ถูกลบและจะเก็บค่าของพวกเขาไว้จนกว่าจะถูกล้างหรือเขียนทับโดยผู้เขียน (โปรดทราบว่า p5 ล้างโดยอัตโนมัติในวง draw) ค่าดีฟอลต์เป็น true 
function setup() { createCanvas(150,150,WEBGL); } function draw() { background(255); push(); rotateZ(frameCount * 0.02); rotateX(frameCount * 0.02); rotateY(frameCount * 0.02); fill(0,0,0); box(50); pop(); }  
ขณะนี้มีแอ็ตทริบิวต์ antialias ตั้งค่าเป็น true 
function setup() { createCanvas(150,150,WEBGL); setAttributes(&#39;antialias&#39;, true); } function draw() { background(255); push(); rotateZ(frameCount * 0.02); rotateX(frameCount * 0.02); rotateY(frameCount * 0.02); fill(0,0,0); box(50); pop(); } 

.. Set attributes for the WebGL Drawing context.
.. This is a way of adjusting ways that the WebGL
.. renderer works to fine-tune the display and performance.
.. This should be put in setup().
.. The available attributes are:
.. 
.. alpha - indicates if the canvas contains an alpha buffer
.. default is true
.. 
.. depth - indicates whether the drawing buffer has a depth buffer
.. of at least 16 bits - default is true
.. 
.. stencil - indicates whether the drawing buffer has a stencil buffer
.. of at least 8 bits
.. 
.. antialias - indicates whether or not to perform anti-aliasing
.. default is false
.. 
.. premultipliedAlpha - indicates that the page compositor will assume
.. the drawing buffer contains colors with pre-multiplied alpha
.. default is false
.. 
.. preserveDrawingBuffer - if true the buffers will not be cleared and
.. and will preserve their values until cleared or overwritten by author
.. (note that p5 clears automatically on draw loop)
.. default is true
.. 
.. 
.. 
.. 
..  function setup() {
..   createCanvas(150,150,WEBGL);
..  }
..  function draw() {
..   background(255);
..   push();
..   rotateZ(frameCount * 0.02);
..   rotateX(frameCount * 0.02);
..   rotateY(frameCount * 0.02);
..   fill(0,0,0);
..   box(50);
..   pop();
..  }
.. 
.. 
.. 
.. Now with the antialias attribute set to true.
.. 
.. 
.. 
..  function setup() {
..   createCanvas(150,150,WEBGL);
..   setAttributes('antialias', true);
..  }
..  function draw() {
..   background(255);
..   push();
..   rotateZ(frameCount * 0.02);
..   rotateX(frameCount * 0.02);
..   rotateY(frameCount * 0.02);
..   fill(0,0,0);
..   box(50);
..   pop();
..  }
.. 
.. 

**รูปแบบการใช้งาน**

setAttributes ( String, New )

**พารามิเตอร์**

- ``String``  String,Object: ชื่อของแอตทริบิวต์หรือวัตถุด้วยคู่คีย์ - ค่า

- ``New``  Boolean: ค่าของแอตทริบิวต์ name

.. ``String``  String,Object: name of attribute or object with key-value pairs
.. ``New``  Boolean: value of named attribute

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
