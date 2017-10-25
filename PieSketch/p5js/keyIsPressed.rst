.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

keyIsPressed
============

คีย์ตัวแปรระบบบูลีนเป็นจริงหากมีการกดปุ่มใด ๆ และเท็จหากไม่มีการกดปุ่มใด ๆ

.. The boolean system variable keyIsPressed is true if any key is pressed and false if no keys are pressed.

**รูปแบบการใช้งาน**

keyIsPressed

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var value = 0;
    function draw() {
        if (keyIsPressed === true) {
            fill(0);
        } else {
            fill(255);
        }
        
        rect(25, 25, 50, 50);
    }
	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
