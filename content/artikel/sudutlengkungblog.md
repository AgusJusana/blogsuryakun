+++
title = "NgeShare - Cara Buat Sudut Lengkung Pada Blog"
date = 2012-11-14T17:25:00Z
tags = ["tutorial", "blogger"]
comments = true
+++

<center><img border="0" data-original-height="600" data-original-width="1200" src="https://4.bp.blogspot.com/-lLfYVwixjc8/XHMLe4HCYQI/AAAAAAAATMI/XFhrmBeyciYClW7ykpRWNUUsSDLwcARIQCLcBGAs/s1600/roundedcorners.png" /></center><br />
<div style="text-align: justify;">Kali ini saya akan membagikan tips bagaimana membuat tampilan pada sudut blogmu menjadi lengkung atau bisa dibilang "rounded corners"<i>. </i>Caranya mudah, kamu hanya perlu menyisipkan kode di bawah ini ke dalam elemen template blogmu. Penerapannya, misalnya saya ingin membuat tampilan sudut "main-wrapper" blog saya menjadi melengkung. Yang harus saya lakukan adalah masuk ke halaman Blogger -&gt; kemudian pilih Template -&gt; Edit HTML.<br /><br />
Dikarenakan saya akan merubah tampilan sudut "main-wrapper" blog saya menjadi melengkung, maka yang harus saya cari adalah kode HTML <span style="color: #cc0000;"><b>#main-wrapper</b></span><b><span style="color: #cc0000;"> {</span></b>, agar lebih cepat untuk menemukan kode tersebut kita tekan tombol CTRL+F pada keyboard. Jika sudah ketemu kode #main-wrapper {, kita sisipkan kode di bawah ini setelah atau di bawah kode <b><span style="color: #cc0000;">#main-wrapper {</span></b>:<br />
<pre><code>border-radius: <span style="color: white;"><span style="background-color: #0b5394;">15px</span></span>;</code></pre><br />
Untuk kode yang ditandai dengan warna biru menunjukkan besaran atau ukuran dari kelengkungan sudut yang dibuat. Semakin besar angka yang dimasukkan, maka akan semakin lengkung sudut yang dibuat, dan itu dapat kamu atur sesuai dengan keinginanmu.<br /><br />
<div style="text-align:center;"><ul class="button"><li><a class="demo" href="https://codepen.io/suryacodekun/pen/LaPRVy" rel="nofollow noopener" target="_blank">Result</a></li></ul></div></div>
