+++
title = "NgeShare - Install Linux Kernel 3.6.3 di Ubuntu 12.10/12.04/Linux Mint 13"
date = 2012-10-24T13:06:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="900" data-original-width="1600" src="https://4.bp.blogspot.com/-vD0Tkh9F008/W-7IYmoAZeI/AAAAAAAASaM/kb5SFGWHncQUDsEne1HIImqSCAo4evW7ACLcBGAs/s1600/linuxkernel.jpg" /></center><br />
<div style="text-align: justify;">Linux kernel 3.6.3 telah dirilis baru-baru ini, versi terbaru ini membawa perubahan dan perbaikan bug. Berikut adalah beberapa perubahan dalam kernel terbaru:<br />
<blockquote class="tr_bq">• PCI INTx eventfd pengaturan telah dipindahkan sebelumnya;<br />• PCI INTx menonaktifkan konsistensi telah diperbaiki;<br />• Delegasi Bad selama pemulihan terbuka telah dihapus;<br />• Jack deteksi pada speaker internal untuk Realtek telah diperbaiki;<br />• Ambang badai EPG sekarang menjadi parameter modul;<br />• CPU / DDR frekuensi perhitungan untuk SRIF PLLs telah diperbaiki;<br />• perulangan tak berujung antara kaskade () dan internal_add_timer () telah diperbaiki;<br />• wthresh perlu diubah menjadi 1 untuk menghindari warung yang mungkin Tx;<br />• Sikap tegas Kegagalan dalam kode komit karena kurang kredit transaksi, telah diperbaiki;<br />• CDC-ACM dukungan untuk Modem CX93010-2x USB UCMxx telah ditambahkan;<br />• set eksplisit dari cache_dynamic_acls = 1 untuk TPG demo-mode telah ditambahkan;<br />• Pemotongan data modus telah diperbaiki dan nol panjang alokasi kini didukung;<br />• per-net NSM klien penciptaan dan penghancuran pembantu telah diperkenalkan;<br />• Pengguna korupsi memori (userland i386 di amd64 kernel) telah diperbaiki;<br />• LPIB delay mengandalkan hardware rusak telah dihentikan;<br />• Sebuah BUG_ON berguna yang menyebabkan kemunduran dalam 3,5 telah diperbaiki</blockquote><br />
Untuk changelog lengkap, klik <b><a href="http://goo.gl/w16BL"><span style="color: #0b5394;">di sini</span></a></b>. Saya akan membantu Anda menginstal Linux Kernel 3.6.3 di Linux distro berikut:<br />
<ul style="text-align: justify;"><li>Ubuntu 12.10/12.04/11.10</li><li>Linux Mint 13/12</li></ul><br /><br />
<b>Instal Linux Kernel 3.6.3</b><<br />
Buka terminal dan isi terminal dengan perintah:<br />
<pre><code>cd /tmp<br /><br />wget http://dl.dropbox.com/u/47950494/upubuntu.com/linux-kernel-3.6.3 -O linux-kernel-3.6.3<br /><br />chmod +x linux-kernel-3.6.3<br /><br />sudo sh linux-kernel-3.6.3</code></pre><br />
Ketika Anda selesai, restart komputer Anda, kemudian periksa kernel dengan perintah ini:<br />
<pre><code>uname -r<br /></code></pre><br />
Bila terjadi kasus kernel ini tidak kompatibel dengan hardware sistem Anda, Anda dapat kembali ke kernel sebelumnya dengan menguninstall versi 3.6.3 dengan perintah ini:<br />
<pre><code>sudo apt-get purge linux-image-3.6.3-030603<br /></code></pre></div>
