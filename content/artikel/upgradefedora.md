+++
title = "NgeShare - Cara Upgrade Fedora 18"
date = 2013-01-27T06:00:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="187" data-original-width="200" src="https://3.bp.blogspot.com/-QwUCLEXbXrU/W--TDCcCmqI/AAAAAAAASdY/h_ZoDLBVtMkNARyG99NRnQFHAP2AIszjACLcBGAs/s1600/fedora.jpg" /></center><br />
<div style="text-align: justify;">Fedora telah merilis versi terbarunya, yaitu versi 18 pada tanggal 15 Januari 2013. Rilis versi 18 ini membawa beberapa perbaikan dan perubahan pada tampilan fedora versi sebelumnya. Jika Anda adalah seorang pengguna Fedora dan Anda ingin meng-upgrade Fedora Anda ke versi 18, berikut ini cara yang akan saya berikan untuk membantu Anda. Mari kita simak! 😁<br /><br />
Sebelum memulai upgrade, silahkan backup data penting sebelum memulai upgrade. Anda dapat meng-upgrade dengan menggunakan fedup.<br />
1. Instal versi terbaru:<br />
<pre><code>yum --enablerepo=updates-testing install fedup</code></pre><br />
Sekarang Anda dapat meng-upgrade dengan menggunakan salah satu dari dua metode di bawah ini:<br />
2-1 Dengan menggunakan jaringan<br />
<pre><code>sudo fedup-cli --network 18 --debuglog fedupdebug.log</code></pre><br />
2-2 Dengan menggunakan file iso<br />
Unduh file iso ke komputer Anda kemudian jalankan perintah pada terminal:<br />
<pre><code>sudo fedup-cli --iso /home/user/fedora-18.iso --debuglog=fedupdebug.log</code></pre><br />
<center><img border="0" src="https://4.bp.blogspot.com/-bcOACiOKMP8/UQRf6g68GzI/AAAAAAAABKI/Xb4OmZkEmiQ/s1600/fedora-18.jpg" /></center></div>
