.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

save()
======

Save an image, text, json, csv, wav, or html. Prompts download to
 the client's computer. Note that it is not recommended to call save()
 within draw if it's looping, as the save() function will open a new save
 dialog every frame.
 The default behavior is to save the canvas as an image. You can
 optionally specify a filename.
 For example:
 
 save();
 save('myCanvas.jpg'); // save a specific canvas with a filename
 
 Alternately, the first parameter can be a pointer to a canvas
 p5.Element, an Array of Strings,
 an Array of JSON, a JSON object, a p5.Table, a p5.Image, or a
 p5.SoundFile (requires p5.sound). The second parameter is a filename
 (including extension). The third parameter is for options specific
 to this type of object. This method will save a file that fits the
 given paramaters. For example:
 
 save('myCanvas.jpg');           // Saves canvas as an image
 var cnv = createCanvas(100, 100);
 save(cnv, 'myCanvas.jpg');      // Saves canvas as an image
 var gb = createGraphics(100, 100);
 save(gb, 'myGraphics.jpg');      // Saves p5.Renderer object as an image
 save(myTable, 'myTable.html');  // Saves table as html file
 save(myTable, 'myTable.csv',);  // Comma Separated Values
 save(myTable, 'myTable.tsv');   // Tab Separated Values
 save(myJSON, 'my.json');        // Saves pretty JSON
 save(myJSON, 'my.json', true);  // Optimizes JSON filesize
 save(img, 'my.png');            // Saves pImage as a png image
 save(arrayOfStrings, 'my.txt'); // Saves strings to a text file with line
                                 // breaks after each item in the array
 

**รูปแบบการใช้งาน**

save ( [objectOrFilename], [filename], [options] )

**พารามิเตอร์**

- ``objectOrFilename``  Object,String: If filename is provided, will save canvas as an image with either png or jpg extension depending on the filename. If object is provided, will save depending on the object and filename (see examples above).

- ``filename``  String: If an object is provided as the first parameter, then the second parameter indicates the filename, and should include an appropriate file extension (see examples above).

- ``options``  Boolean,String: Additional options depend on filetype. For example, when saving JSON, <code>true</code> indicates that the output will be optimized for filesize, rather than readability.


.. toctree::

