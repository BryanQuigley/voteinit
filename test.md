---
layout: page
title: Test
permalink: /test/
---



<p>Click on the button to copy the text from the text field. Try to paste the text (e.g. ctrl+v) afterwards in a different window, to see the effect.</p>


<textarea rows="5" cols="80" id="myInput">
The changing of the clock every Spring is deadly, with heart attacks, strokes, traffic accidents and workplace accidents all spiking. The change is disruptive to business, painful for families, and difficult for millions. It's a legitimate public health crisis. Please do whatever you can to help end the clock changing. Thank you very much.
</textarea>
<button onclick="myFunction()">Copy This and Go to democracy.io to contact your reps (paste it there)</button>


<script>
function myFunction() {
  var copyText = document.getElementById("myInput");
  copyText.select();
  copyText.setSelectionRange(0, 99999)
  document.execCommand("copy");
  var win = window.open("https://democracy.io/", '_blank');
  win.focus();
  //alert("Copied the text: " + copyText.value);
}
</script>