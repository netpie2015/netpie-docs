.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

save()
======

 บันทึกรูปภาพข้อความ json, csv, wav หรือ html พร้อมท์ให้ดาวน์โหลดไปยังคอมพิวเตอร์ของลูกค้า โปรดทราบว่าไม่แนะนำให้เรียกบันทึก () ภายในการวาดถ้าเป็นลูปเนื่องจากฟังก์ชัน save () จะเปิดกรอบโต้ตอบการบันทึกใหม่ทุกเฟรม  ลักษณะการทำงานเริ่มต้นคือการบันทึกผืนผ้าใบเป็นรูปภาพ คุณสามารถระบุชื่อไฟล์ได้ ตัวอย่างเช่น:  save(); save(&#39;myCanvas.jpg&#39;); // save a specific canvas with a filename  อีกวิธีหนึ่งคือพารามิเตอร์ตัวแรกอาจเป็นตัวชี้ไปยัง p5.Element บนผ้าใบอาร์เรย์ของสตริงอาร์เรย์ของ JSON ออบเจ็กต์ JSON p5.Table p5.Image หรือ p5.SoundFile (ต้องใช้ p5.sound ) พารามิเตอร์ที่สองคือชื่อไฟล์ (รวมถึงส่วนขยาย) พารามิเตอร์ที่สามใช้สำหรับตัวเลือกเฉพาะสำหรับประเภทของอ็อบเจ็กต์นี้ วิธีนี้จะบันทึกไฟล์ที่เหมาะกับพาเรเตอร์ที่ระบุ ตัวอย่างเช่น:  save(&#39;myCanvas.jpg&#39;); // Saves canvas as an image var cnv = createCanvas(100, 100); save(cnv, &#39;myCanvas.jpg&#39;); // Saves canvas as an image var gb = createGraphics(100, 100); save(gb, &#39;myGraphics.jpg&#39;); // Saves p5.Renderer object as an image save(myTable, &#39;myTable.html&#39;); // Saves table as html file save(myTable, &#39;myTable.csv&#39;,); // Comma Separated Values save(myTable, &#39;myTable.tsv&#39;); // Tab Separated Values save(myJSON, &#39;my.json&#39;); // Saves pretty JSON save(myJSON, &#39;my.json&#39;, true); // Optimizes JSON filesize save(img, &#39;my.png&#39;); // Saves pImage as a png image save(arrayOfStrings, &#39;my.txt&#39;); // Saves strings to a text file with line // breaks after each item in the array 

.. Save an image, text, json, csv, wav, or html. Prompts download to
..  the client's computer. Note that it is not recommended to call save()
..  within draw if it's looping, as the save() function will open a new save
..  dialog every frame.
..  The default behavior is to save the canvas as an image. You can
..  optionally specify a filename.
..  For example:
..  
..  save();
..  save('myCanvas.jpg'); // save a specific canvas with a filename
..  
..  Alternately, the first parameter can be a pointer to a canvas
..  p5.Element, an Array of Strings,
..  an Array of JSON, a JSON object, a p5.Table, a p5.Image, or a
..  p5.SoundFile (requires p5.sound). The second parameter is a filename
..  (including extension). The third parameter is for options specific
..  to this type of object. This method will save a file that fits the
..  given paramaters. For example:
..  
..  save('myCanvas.jpg');           // Saves canvas as an image
..  var cnv = createCanvas(100, 100);
..  save(cnv, 'myCanvas.jpg');      // Saves canvas as an image
..  var gb = createGraphics(100, 100);
..  save(gb, 'myGraphics.jpg');      // Saves p5.Renderer object as an image
..  save(myTable, 'myTable.html');  // Saves table as html file
..  save(myTable, 'myTable.csv',);  // Comma Separated Values
..  save(myTable, 'myTable.tsv');   // Tab Separated Values
..  save(myJSON, 'my.json');        // Saves pretty JSON
..  save(myJSON, 'my.json', true);  // Optimizes JSON filesize
..  save(img, 'my.png');            // Saves pImage as a png image
..  save(arrayOfStrings, 'my.txt'); // Saves strings to a text file with line
..                                  // breaks after each item in the array
..  
**รูปแบบการใช้งาน**

save ( [objectOrFilename], [filename], [options] )

**พารามิเตอร์**

- ``objectOrFilename``  Object,String: หากมีชื่อไฟล์ไว้จะบันทึกภาพเป็นภาพที่มีนามสกุล png หรือ jpg ขึ้นอยู่กับชื่อไฟล์ ถ้ามีการจัดเก็บวัตถุจะบันทึกขึ้นอยู่กับวัตถุและชื่อไฟล์ (ดูตัวอย่างด้านบน)

- ``filename``  String: หากมีการระบุออบเจ็กต์เป็นพารามิเตอร์แรกพารามิเตอร์ที่สองจะระบุชื่อไฟล์และควรมีส่วนขยายไฟล์ที่เหมาะสม (ดูตัวอย่างด้านบน)

- ``options``  Boolean,String: ตัวเลือกเพิ่มเติมขึ้นอยู่กับชนิดของไฟล์ ตัวอย่างเช่นเมื่อบันทึก JSON <code>true</code> แสดงว่าเอาต์พุตจะได้รับการปรับให้เหมาะกับขนาดไฟล์แทนที่จะอ่านได้

.. ``objectOrFilename``  Object,String: If filename is provided, will
                                            save canvas as an image with
                                            either png or jpg extension
                                            depending on the filename.
                                            If object is provided, will
                                            save depending on the object
                                            and filename (see examples
                                            above).
.. ``filename``  String: If an object is provided as the first
                              parameter, then the second parameter
                              indicates the filename,
                              and should include an appropriate
                              file extension (see examples above).
.. ``options``  Boolean,String: Additional options depend on
                           filetype. For example, when saving JSON,
                           <code>true</code> indicates that the
                           output will be optimized for filesize,
                           rather than readability.

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
