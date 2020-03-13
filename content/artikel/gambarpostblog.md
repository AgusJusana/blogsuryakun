+++
title = "NgeShare - Membuat Efek Bayangan pada Gambar di Posting Blog"
date = 2012-08-02T15:15:00Z
tags = ["tutorial", "blogger"]
comments = true
+++

<center><img border="0" data-original-height="600" data-original-width="1200" src="https://3.bp.blogspot.com/-lFOcVtHu2Ag/XHMq0rVfRDI/AAAAAAAATMQ/BobO9wxII0ArSsy_Ph4LDqG1g6R6FPw_wCLcBGAs/s1600/box.png" /></center><br />
<div style="text-align: justify;">Pada kesempatan kali ini, saya akan memberikan tutorial untukmu yang ingin membuat atau memberikan efek bayangan pada gambar di postingan blogmu. Oke langsung saja kita simak tutorialnya berikut ini.<br /><br />
1. Login ke Blogger<br />
2. Pada halaman Dashboard pilih menu "Tema"<br />
3. Kemudian kamu tekan tombol "Edit HTML"<br />
4. Pada fitur "Edit HTML", kamu cari kode <span style="color: #0b5394;"><b>.post-body img</b></span><b><span style="color: #0b5394;"></span></b><br />
5. Kemudian kamu tambahkan kode di bawah ini ke dalam elemen kode<b><span style="color: #0b5394;"> </span></b><span style="color: #0b5394;"><b>.post-body img</b></span><br />
- Kode box shadow (normal)<br /><pre><code class="language-css">box-shadow: 0 2px 4px 0 rgba(0,0,0,0.10);</code></pre><br />
- Kode box shadow-md (medium)<br /><pre><code class="language-css">box-shadow: 0 4px 8px 0 rgba(0,0,0,0.12), 0 2px 4px 0 rgba(0,0,0,0.08);</code></pre><br />
- Kode box shadow-lg (large)<br /><pre><code class="language-css">box-shadow: 0 15px 30px 0 rgba(0,0,0,0.11), 0 5px 15px 0 rgba(0,0,0,0.08);</code></pre><br />
- Kode box shadow-inner<br /><pre><code class="language-css">box-shadow: inset 0 2px 4px 0 rgba(0,0,0,0.06);</code></pre><br />
- Kode box shadow-outline<br /><pre><code class="language-css">box-shadow: 0 0 0 3px rgba(52,144,220,0.5);</code></pre><br /><br />
Contoh pemasangan:<br /><pre><code class="language-css">.post-body img {<br />padding: 1px;<br />background: transparent;<br />border: 2px solid transparent;<br />box-shadow: 0 2px 4px 0 rgba(0,0,0,0.10);<br />}</code></pre><br />6. &nbsp;Lalu Anda klik Simpan<br /><div style="text-align:center;"><ul class="button"><li><a class="demo" href="https://codepen.io/suryacodekun/full/VRZPwL" rel="nofollow noopener" target="_blank">Result</a></li></ul></div></div>
