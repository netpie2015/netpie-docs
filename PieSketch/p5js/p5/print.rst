.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

print()
=======

ฟังก์ชัน print () เขียนลงในพื้นที่คอนโซลของเบราเซอร์ของคุณ ฟังก์ชันนี้มักจะเป็นประโยชน์สำหรับการดูข้อมูลที่โปรแกรมกำลังผลิตอยู่ ฟังก์ชันนี้จะสร้างบรรทัดใหม่ของข้อความสำหรับการโทรแต่ละครั้งไปยังฟังก์ชัน แต่ละองค์ประกอบสามารถคั่นด้วยเครื่องหมายคำพูด (&quot;&quot;) และเชื่อมต่อกับโอเปอเรเตอร์ add (+) 
ในขณะที่ print () มีลักษณะคล้ายกับ console.log () ไม่ตรงไปตรงมาเพื่อจำลองพฤติกรรมให้เข้าใจง่ายกว่า console.log () ด้วยเหตุนี้มันจึงช้าลง เพื่อผลลัพธ์ที่เร็วที่สุดให้ใช้ console.log ()

.. The print() function writes to the console area of your browser.
.. This function is often helpful for looking at the data a program is
.. producing. This function creates a new line of text for each call to
.. the function. Individual elements can be
.. separated with quotes ("") and joined with the addition operator (+).
.. 
.. While print() is similar to console.log(), it does not directly map to
.. it in order to simulate easier to understand behavior than
.. console.log(). Due to this, it is slower. For fastest results, use
.. console.log().
**รูปแบบการใช้งาน**

print ( contents )

**พารามิเตอร์**

- ``contents``  Any: การรวมกันของ Number, String, Object, Boolean, Array เพื่อพิมพ์

.. ``contents``  Any: any combination of Number, String, Object, Boolean,
                      Array to print

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	<code class='norender'>
	var x = 10;
	print("The value of x is " + x);
	// prints "The value of x is 10"

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
