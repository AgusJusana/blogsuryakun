+++
title = "NgeShare - Cara Reinstall/ Perbaikan GRUB 2 Bootloader di Ubuntu 12.10/12.04"
date = 2012-11-24T16:07:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<div style="text-align: justify;">Dalam tutorial ini, saya akan menunjukkan kepada Anda bagaimana menggunakan utilitas&nbsp;<b>Boot Repair&nbsp;</b>untuk memperbaiki boot loader G<b>rub 2</b> di Ubuntu/ Linux Mint.&nbsp;<b>Boot Repair</b>&nbsp;berguna bagi pengguna yang mengalami masalah booting yang terjadi terutama ketika dual-boot Ubuntu dengan sistem operasi lain seperti Windows 8/7, dll. Anda juga dapat menggunakannya untuk menginstal ulang Grub 2 bila Anda memiliki boot loader yang telah&nbsp;terkonfigurasi. Untuk memulia tutorial ini, Anda harus memenuhi beberapa persyaratan berikut ini:<br /><br />
<ul><li>Ubuntu Live CD / USB (Ubuntu 12.10/12.04)</li><li>Koneksi Internet</li></ul><br /><br />

<b>1. Boot dari Live CD / USB</b><br />
Boot ke live CD/ USB&nbsp;Anda,&nbsp;dari layar pertama Anda pilih "<b>Try Ubuntu without installing</b>":<br />
<center><img border="0" src="https://1.bp.blogspot.com/-TtB1aVQaMfM/ULCL9i88MlI/AAAAAAAAAH4/Dd5mZRLbDUM/s1600/try.png" /></center><br />
Kemudian tunggu hingga desktop Anda muncul sepenuhnya.<br /><br />
<b>2. Instal Boot Repair</b><br />
Buka terminal dan masukkan perintah di bawah ini:<br />
<pre><code>sudo add-apt-repository ppa:yannubuntu/boot-repair<br />sudo apt-get update<br />sudo apt-get install boot-repair boot-sav</code></pre><br />
<b>3. Memperbaiki / Menginstal ulang grub2</b><br />
Sekarang Anda dapat mulai Boot-Repair dengan perintah ini:<br />
<pre><code>boot-repair</code></pre><br />
Dari antarmuka utama aplikasi, klik "<b>Recommended repair (...)</b>":<br />
<center><img border="0" src="https://2.bp.blogspot.com/-fcGKn4td9fg/ULCNH52U2sI/AAAAAAAAAIA/eDlOhspymh4/s1600/try2.png" /></center><br />
Untuk pengguna tingkat lanjut, Anda bisa mengklik "<b>Advanced options</b>" untuk tindakan lebih (mengembalikan MBR, memperbaiki sistem file, perubahan standar OS, dll):<br />
<center><img border="0" src="https://1.bp.blogspot.com/-vXdBJcTC1Hg/ULCNh7TXi-I/AAAAAAAAAII/YPCyFzvEcio/s1600/try3.png" /></center><br />
<center><img border="0" src="https://1.bp.blogspot.com/-iUsvbEKMVQs/ULCNmClm-EI/AAAAAAAAAIQ/FYHiQPToo70/s1600/try4.png" /></center><br />
Jika perbaikan berhasil, Anda akan mendapatkan pesan ini:<br />
<center><img border="0" src="https://3.bp.blogspot.com/-Q-oOF0GGUYU/ULCN3j_bfWI/AAAAAAAAAIY/MnMubb6Vl64/s1600/try5.png" /></center><br />
Dan terakhir, reboot sistem Anda untuk menyelesaikannya.</div>
