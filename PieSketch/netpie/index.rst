.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

NETPIE
======

`NETPIE <https://netpie.io>`_ เป็นบริการคลาวด์สำหรับการพัฒนา IOT application บนหลากหลาย platform ไม่ว่าจะเป็น hardware, software, หรือ web application สำหรับ PieSketch ก็จัดเป็นอีกหนึ่ง platform ที่ NETPIE ให้บริการด้วยเช่นกัน การเริ่มต้นใช้งาน PieSketch กับ NETPIE ท่านต้องเริ่มต้นจากการสมัครสมาชิก และสร้าง App ID, Key, Secret `[ตามขั้นตอนนี้] <https://www.gitbook.com/book/netpie/doc/details>`_  ในส่วนของการพัฒนา hardware IOT ท่านสามารถศึกษาได้ด้วยตัวเองจาก `[คู่มือ NETPIE] <https://www.gitbook.com/@netpie>`_ แต่ในที่นี้ เราจะกล่าวถึงเฉพาะการพัฒนาบน PieSketch เท่านั้น ซึ่ง PieSketch แต่ละ project ที่เชื่อมต่อเข้ากับ NETPIE รวมถึง hardware ที่ต่อ NETPIE อยู่แล้ว สามารถทำงานร่วมกันได้ทั้งหมด

.. note::
	ก่อนจะใช้งาน NETPIE ท่านต้องทำการสร้าง account ที่ https://netpie.io และ activate account ให้เรียบร้อย และทำการสร้าง App ID, Key, Secret แนะนำให้สร้าง Key ชนิด session key สำหรับใช้กับ PieSketch

Microgear
---------

การเชื่อมต่อกับ NETPIE จะทำผ่านฟังก์ชั่นของ Microgear library หรือพูดอีกนัยหนึ่งก็คือ การใช้งาน NETPIE ก็คือการออกแบบสร้่าง microgear ขึ้นมาทำงานร่วมกันนั่นเอง สำหรับ PieSketch ก็มีตัวแปรชนิด Microgear ให้เรียกใช้ ซึ่งจะมาพร้อมคำสั่งดังนี้


- :ref:`create() <create>`
- :ref:`connect() <connect>`
- :ref:`setAlias() <setAlias>`
- :ref:`chat() <chat>`
- :ref:`publish() <publish>`
- :ref:`subscribe() <subscribe>`
- :ref:`unsubscribe() <unsubscribe>`

----

.. _create:

create()
--------

เป็นการสร้างตัวแปร microgear โดยใช้คำสั่ง creat ดังนี้

.. code-block:: javascript

	Microgear.create ( key, secret, [alias] )

- ``key``  String: เป็นค่า key ที่ได้มาจากการเว็บ netpie.io

- ``secret``  String: เป็น secret ของ key ซึ่งจะใช้ประกอบในกระบวนการยืนยันตัวตน 

- ``alias``  String: ชื่อเล่นของ microgear ตัวนี้ สำหรับให้ microgear อื่นอ้างอิงถึง สามารถตั้งทีหลังในโค้ดได้

**ค่าที่ส่งออกมา**

- microgear : ตัวแปรชนิด microgear

.. code-block:: javascript
	:caption: ตัวอย่างการใช้งาน

	var microgear = Microgear.create({
		key: 'M5AT1tW3oEgilr7',
		secret: 'SenjBILrRd4a4coNX8mb9exMT',
		alias:'p5js'
	});

----

.. _connect:

connect()
---------

การเชื่อมต่อ NETPIE จะเกิดขึ้นก็ต่อเมื่อเราสั่งให้ microgear ทำการเชื่อมต่อ โดยใช้คำสั่ง

.. code-block:: javascript

	microgear.connect ( appid )

- ``appid``  String: เป็นค่า App ID เป้าหมายที่จะเชื่อมต่อเข้าไป

.. code-block:: javascript
	:caption: ตัวอย่างการใช้งาน

	microgear.connect("happyfarm");

.. warning::
	การเชื่อมต่อ จะใช้ port  8081 และ 8084 กรุณาตรวจสอบว่าเครือข่ายของท่านอนุญาตให้ใช้งานได้

----

.. _setAlias:

setAlias()
----------

หากไม่ได้ตั้งชื่อไว้ตอนที่สร้าง เราก็ยังสามารถเปลี่ยนชื่อตัวเองได้ตลอดเวลา

.. code-block:: javascript

	microgear.connect ( alias )

- ``alias``  String: ชื่อของ microgear อันนี้

.. code-block:: javascript
	:caption: ตัวอย่างการใช้งาน

	microgear.setAlias("plant");

.. note::
	ใน App ID เดียวกัน เราสามารถตั้งชื่อ alias เดียวกันให้กับหลาย microgear พร้อมๆกันได้ และใน App ID ที่ต่างกัน ชือ alias ถึงแม้จะซ้ำกันก็จะไม่มีผลถึงกัน

----

.. _chat:

chat()
----------

ส่งข้อความไปยัง microgear ที่มีชื่อตามที่ระบุ

.. code-block:: javascript

	microgear.chat ( alias , message)

- ``alias``  String: ชื่อของ microgear อันนี้

- ``message``  String|Number|Object: ข้อความที่จะส่งไป


.. code-block:: javascript
	:caption: ตัวอย่างการใช้งาน

	microgear.chat("valve","I need water");

----

.. _publish:

publish()
----------

ในการณีที่ต้องการส่งข้อความแบบไม่เจาะจงผู้รับ สามารถใช้ฟังชั่น publish ไปยัง topic ที่กำหนดได้ ซึ่งจะมีแต่ microgear ที่ subscribe topoic นี้เท่านั้น ที่จะได้รับข้อความ

ส่งข้อความไปยัง microgear ที่มีชื่อตามที่ระบุ

.. code-block:: javascript

	microgear.publish ( topic , message )

- ``alias``  String: ชื่อของ topic ที่ต้องการจะส่งข้อความไปถึง 

- ``message``  String|Number|Object: ข้อความที่จะส่งไป


.. code-block:: javascript
	:caption: ตัวอย่างการใช้งาน

	microgear.publish("/outdoor/temp","28.5");

----

.. _subscribe:

subscribe()
-----------

microgear อาจจะมีความสนใจใน topic ใดเป็นการเฉพาะ เราสามารถใช้ฟังก์ชั่น subscribe() ในการบอกรับ message ของ topic นั้นได้

.. code-block:: javascript

	microgear.subscribe ( topic )

- ``alias``  String: ชื่อของ topic ที่สนใจต้องการรับข้อความ 


.. code-block:: javascript
	:caption: ตัวอย่างการใช้งาน

	microgear.subscribe("/outdoor/temp");

.. note::
	นอกจากการระบุ topic เป็น string แบบชัดเจนแล้ว เรายังสามารถใช้สัญลักษณ์ wildcard เครื่องหมาย # และ * ได้ด้วย ศึกษาเพิ่มเติมได้ที่นี่ `[wildcard] <wildcard.html>`_


----












