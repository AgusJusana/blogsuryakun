+++
title = "NgeShare - Cara Ganti DNS di Ubuntu"
date = 2014-01-11T16:36:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="600" data-original-width="1200" src="https://4.bp.blogspot.com/-_VSiv3-90H4/XF3yOIBwxVI/AAAAAAAATHg/1Hlr6jgwCC4ECgwmtcgpURFKroyCeysugCLcBGAs/s1600/dns.png" /></center><br />
<div style="text-align: justify;">Kali ini gue mau ngeshare artikel tentang cara mengganti DNS di Ubuntu. Gimana caranya? Mari disimak langkah-langkah di bawah ini.<br /><br />
1. Pastikan kamu sudah masuk ke koneksi internet melalui modem.<br />
2. Kemudian kamu buka terminal atau tekan tombol <b>CTRL+ALT+T</b>.<br />
<center><img border="0" height="406" src="https://4.bp.blogspot.com/-R4vmrWIASy4/Us_ZOPCyToI/AAAAAAAAD8I/qrOkMgfmncQ/s1600/1.jpg" width="640" /></center><br />
3. Kalau terminalnya udah muncul, lalu masukkan perintah di bawah ini. Terus tekan tombol <b>Enter</b>.<br />
<pre class="CSS" name="code"><code>sudo nano /etc/resolv.conf</code></pre><br />
<center><img border="0" height="406" src="https://1.bp.blogspot.com/-aoj0_Gw5Cjs/Us_aLv1oPxI/AAAAAAAAD8Q/i9fq5KDhcq0/s1600/2.jpg" width="640" /></center><br />
4. Munculah tampilan baru seperti gambar di bawah ini.<br />
<center><img border="0" height="406" src="https://3.bp.blogspot.com/-WT4Xcp51F7c/Us_axKVM8JI/AAAAAAAAD8Y/LSXX8zVIVKg/s1600/3.jpg" width="640" /></center><br />
5. Kamu fokus sama 2 nameserver di atas. Pada 2 nameserver tersebut, kamu beri tanda <b>pagar (#)</b> di depannya.<br />
<center><img border="0" height="406" src="https://3.bp.blogspot.com/-dzBuChggeyI/Us_cL77BD8I/AAAAAAAAD8k/IjZHRUc-mq8/s1600/4.jpg" width="640" /></center><br />
6. Setelah kamu beri tanda pagar pada setiap nameserver tersebut, kamu buat 2 nameserver baru di atasnya. Yang paling atas atau pertama <b>nameserver 8.8.8.8</b>, yang kedua <b>nameserver 8.8.4.4</b>.<br />
<center><img border="0" height="406" src="https://4.bp.blogspot.com/-jGLlIT-j68o/Us_dpWx2uYI/AAAAAAAAD8w/KOGDxPXbm5I/s1600/5.jpg" width="640" /></center><br />
7. Kalau udah buat 2 nameserver, kamu simpan dengan menekan tombol <b>CTRL+O</b>, lalu kamu tekan tombol <b>Enter</b>.<br />
8. Kemudian kamu keluar dari tampilan di atas dengan menekan tombol <b>CTRL+X </b>pada keyboard.<br /><br />
Nah, DNS kamu berhasil kamu ganti.<br /><br />
Biasanya penggantian DNS ini dilakukan ketika terjadi masalah pada koneksi internet kita, khususnya koneksi internet pada modem. Misalnya tidak dapat memuat suatu halaman website atau blank page. Untuk itu bila kamu menemukan masalah tersebut dan kamu menggunakan Ubuntu, maka cobalah langkah-langkah yang gue publikasikan ini.<br /><br />
Semoga bermanfaat. :)</div>
