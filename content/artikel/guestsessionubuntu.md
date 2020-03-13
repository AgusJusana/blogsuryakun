+++
title = "NgeShare - Menyembunyikan Guest Session Saat Login di Ubuntu 13.04"
date = 2013-06-20T05:20:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="600" data-original-width="1200" src="https://2.bp.blogspot.com/-AbkQBdLodZw/XF30OqWkdSI/AAAAAAAATH4/xxxNsGdGZBUIQMvIh4X6ao1QktkVebZpgCLcBGAs/s1600/guest.png" /></center><br />
<div style="text-align: justify;">Pada kesempatan ini, saya akan membagikan sebuah tips bagaimana cara menyembunyikan Guest Session pada saat login di Ubuntu 13.04. Sebelumnya Anda pasti telah tahu apa itu Guest Session kan? Guset Session adalah sebuah fitur dalam Ubuntu yang memungkinkan Anda untuk memilih sesi dekstop yang telah terinstal di Ubuntu Anda, seperti misalnya Unity, Gnome XCFE, dan lain-lain.<br />
<center><img border="0" src="https://3.bp.blogspot.com/-scjCZ8MEUZE/UcIt3okaAMI/AAAAAAAACdg/43wgpg46tOo/s1600/2013-06-20+04.55.20.jpg" /></center><br />
Oke kembali lagi dengan tipsnya, tips ini cukup singkat untuk Anda lakukan. Cukup masukkan perintah di bawah ini ke dalam terminal:<br />
<blockquote class="tr_bq">sudo /usr/lib/lightdm/lightdm-set-defaults -l false</blockquote><br />
Kemudian Anda harus logout, gunakan perintah berikut ini:<br />
<blockquote class="tr_bq">sudo restart lightdm</blockquote><br />
Maka hasilnya seperti ini:<br />
<center><img border="0" src="https://4.bp.blogspot.com/-lNI_Rzw5PPQ/UcIuSyGZazI/AAAAAAAACdo/hpF4YBsZEw8/s1600/2013-06-20+05.01.31.jpg" /></center><br />
Jika Anda ingin menampilkan kembali Guest Session, cukup gunakan perintah:<br />
<blockquote class="tr_bq">sudo /usr/lib/lightdm/lightdm-set-defaults -l true</blockquote><br />
Dan kemudian Anda logout:<br />
<blockquote class="tr_bq">sudo restart lightdm </blockquote></div>
