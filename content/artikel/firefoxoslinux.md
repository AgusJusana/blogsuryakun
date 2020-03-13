+++
title = "NgeShare - Mencoba Firefox OS di Linux Ubuntu"
date = 2012-08-03T02:58:00Z
tags = ["tutorial", "linux", "teknologi"]
comments = true
+++

<center><img border="0" data-original-height="900" data-original-width="1600" src="https://4.bp.blogspot.com/-og1sfbT8iyw/W-t8R_mnYqI/AAAAAAAASM4/WG9P5Ye7X4YJX6ElA7cs8fuQWSpvSNCzgCLcBGAs/s1600/firefox-os.jpg" /></center><br />
<div style="text-align: justify;">"Firefox", pasti jika Anda mendengar kata tersebut Anda akan berpikir tentang sebuah software peramban web yang bernama lengkap "Mozilla Firefox". Kini Firefox tidak hanya digunakan sebagai sebuah nama software peramban web namun juga digunakan sebagai nama OS smartphone, kok bisa gitu sih?<br /><br />
Ya, bisa-bisa ajalah karena sekarang Mozilla telah membuat dan mengembangkan sebuah OS smartphone yang bernama "Firefox OS". Firefox OS atau yang masih diberi nama kode "Boot to Gecko" ini merupakan OS untuk smartphone yang membawa visi menghadirkan Open Web sebagai platform untuk mobile device. Firefox OS akan memberi kemudahan untukdeveloper dalam membuat aplikasi, kustomisasi untuk penyedia layanan seluler, dan lain-lain. Yaah, mungkin bisa jadi alternatif OS smartphone bagi yang bosan ngoprek Android. Untuk informasi lebih lanjut mengenai Firefox OS, silakan klik <a href="http://www.mozilla.org/en-US/b2g/">di sini</a>.<br />
<table cellpadding="0" cellspacing="0" class="tr-caption-container" style="margin-left: auto; margin-right: auto; text-align: left;"><tbody><tr><td style="text-align: center;"><img src="https://2.bp.blogspot.com/-vMirH_cOp2Q/UAkna9SreRI/AAAAAAAAEC8/OQ00MNC0NK0/s1600/Selection_332.png" style="margin-left: auto; margin-right: auto;" /></td></tr><tr><td class="tr-caption" style="text-align: center;">Firefox OS di Linux Ubuntu</td></tr></tbody></table><br />
<table cellpadding="0" cellspacing="0" class="tr-caption-container" style="margin-left: auto; margin-right: auto; text-align: left;"><tbody><tr><td style="text-align: center;"><img src="https://3.bp.blogspot.com/-pZOPSQZEf4o/UAksOPs-Y5I/AAAAAAAAEDI/pK7qtC4X-jw/s1600/Selection_333.png" style="margin-left: auto; margin-right: auto;" /></td></tr><tr><td class="tr-caption" style="text-align: center;">Menu Utama Firefox OS</td></tr></tbody></table><br />
<span style="font-size: large;"><b>Mencoba Firefox OS di Linux Ubuntu</b></span><br />
Meskipun smartphone berbasis Firefox OS belum beredar, kita dapat mencobanya lebih awal. Ya, dari Ubuntu kita!<br /><br />
<b>Mengunduh Firefox OS</b><br />
Silakan unduh dahulu Firefox OS versi terbaru (latest build) <a href="http://ftp.mozilla.org/pub/mozilla.org/b2g/nightly/latest-mozilla-central/">di sini</a>. Kalian akan menemukan banyak tautan di sana, pilih saja <span style="background-color: #f3f3f3;"><b>b2g-17.0a1.en-US.linux-i686.tar.bz2</b></span> atau versi yang lebih baru.<br /><br />
Setelah proses unduh selesai, ekstrak file sehingga menghasilkan folder yang bernama "b2g". Nah, sekarang silakan buka Terminal dan masuk ke folder "b2g" tersebut, lalu ketik perintah berikut untuk mengunduh dan menginstal Gaia (emulator untuk Firefox OS):<br />
<pre><code>view plainprint?git clone git://github.com/mozilla-b2g/gaia<br />make -C gaia profile</code></pre><br />
Proses ini membutuhkan waktu yang cukup lama karena harus mengunduh file sebanyak ratusan megabyte. Nah, setelah semuanya selesai, ketik perintah berikut untuk menjalankan Firefox OS:<br />
<pre><code>view plainprint?./b2g -profile gaia/profile</code></pre><br />
Oh, iya, Firefox OS ini masih dalam tahap pengembangan, jadi jangan berharap banyak dulu terhadap Firefox OS sekarang.</div>
