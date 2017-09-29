.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

Event
=====

application ที่รันบน microgear จะมีการทำงานในแบบ event-driven คือ การเขียนโปรแกรมเชื่อมต่อ NETPIE จะเป็นการเขียน callback function ขึ้นมาตอบสนองต่อ event ต่างๆ ในลักษณะนี้

.. code-block:: javascript

	microgear.on (*event*, *callback*)

- ``event``  String: ชื่อ event

- ``callback``  Function: callback function ที่จะถูกเรียก บาง event อาจจะส่ง parameter มาให้ด้วย

event ที่เกิดจาก microgear มีดังนี้

- :ref:`connected <connected>`
- :ref:`disconnected <disconnected>`
- :ref:`info <info>`
- :ref:`error <error>`
- :ref:`message <message>`
- :ref:`present <present>`

----



.. _connected:

Event: 'connected'
^^^^^^^^^^^^^^^^^^

เกืดขึ้นเมื่อ microgear library เชื่อมต่อกับ platform สำเร็จ

.. code-block:: javascript
	:caption: ตัวอย่างการใช้งาน

	microgear.on("connected", function() {
		console.log("connected");
	});

----

.. _disconnected:

Event: 'disconnected'
^^^^^^^^^^^^^^^^^^

เกืดขึ้นเมื่อ microgear library ตัดการเชื่อมต่อกับ platform

.. code-block:: javascript
	:caption: ตัวอย่างการใช้งาน

	microgear.on("closed", function() {
		console.log("closed");
	});

----

.. _info:

Event: 'info'
^^^^^^^^^^^^^^^^^^

เป็น event แจ้งข่าวออกมาจาก microgear

.. code-block:: javascript
	:caption: ตัวอย่างการใช้งาน

	microgear.on("info", function(err) {
		console.log("Info: "+err);
	});

----

.. _error:

Event: 'error'
^^^^^^^^^^^^^^^^^^

เป็น event ที่เกิดมี error ขึ้นภายใน microgear

.. code-block:: javascript
	:caption: ตัวอย่างการใช้งาน

	microgear.on("error", function(err) {
		console.log("Error: "+err);
	});

----

.. _message:

Event: 'message'
^^^^^^^^^^^^^^^^^^

เมื่อมี message เข้ามา จะเกิด event นี้ขึ้น พร้อมกับส่งผ่านข้อมูลเกี่ยวกับ message นั้นมาทาง argument ของ callback function

.. code-block:: javascript
	:caption: ตัวอย่างการใช้งาน

	microgear.on("message", function(topic,msg) {
		console.log("Incoming message: "+msg);
	});

----

.. _present:

Event: 'present'
^^^^^^^^^^^^^^^^^^

event นี้จะเกิดขึ้นเมื่อมี microgear ใน appid เดียวกัน online เข้ามาเชื่อมต่อ netpie

.. code-block:: javascript
	:caption: ตัวอย่างการใช้งาน

	microgear.on("present", function(event) {
		console.log("New friend found: "+event.gearkey);
	});
