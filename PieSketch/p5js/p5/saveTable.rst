.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

saveTable()
===========

เขียนเนื้อหาของวัตถุ Table ไปยังแฟ้ม ค่าเริ่มต้นเป็นไฟล์ข้อความที่มีคั่นด้วยเครื่องหมายจุลภาค ('csv') แต่ยังสามารถใช้การแยกแท็บ ('tsv') หรือสร้างตาราง HTML ('html') กระบวนการบันทึกไฟล์และตำแหน่งของไฟล์ที่บันทึกไว้จะแตกต่างกันไปในแต่ละเว็บเบราเซอร์

.. Writes the contents of a Table object to a file. Defaults to a
..  text file with comma-separated-values ('csv') but can also
..  use tab separation ('tsv'), or generate an HTML table ('html').
..  The file saving process and location of the saved file will
..  vary between web browsers.

**รูปแบบการใช้งาน**

saveTable ( Table, filename, [options] )

**พารามิเตอร์**

- ``Table``  p5.Table: วัตถุ Table เพื่อบันทึกลงในไฟล์

- ``filename``  String: ชื่อไฟล์ที่ควรบันทึกตาราง

- ``options``  String: สามารถเป็นหนึ่งใน &quot;tsv&quot;, &quot;csv&quot; หรือ &quot;html&quot;

.. ``Table``  p5.Table: the Table object to save to a file
.. ``filename``  String: the filename to which the Table should be saved
.. ``options``  String: can be one of "tsv", "csv", or "html"

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	 var table;
	
	 function setup() {
	   table = new p5.Table();
	
	   table.addColumn('id');
	   table.addColumn('species');
	   table.addColumn('name');
	
	   var newRow = table.addRow();
	   newRow.setNum('id', table.getRowCount() - 1);
	   newRow.setString('species', 'Panthera leo');
	   newRow.setString('name', 'Lion');
	
	   // To save, un-comment next line then click 'run'
	   // saveTable(table, 'new.csv');
	   }
	
	   // Saves the following to a file called 'new.csv':
	   // id,species,name
	   // 0,Panthera leo,Lion
	 

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
