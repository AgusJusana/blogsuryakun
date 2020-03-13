+++
title = "NgeShare - Cara Menonaktifkan Laporan Apport di Ubuntu 12.04"
date = 2012-08-16T19:06:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<div style="text-align: justify;">Bagi kamu pengguna Linux Ubuntu 12.04 yang mungkin pernah mendapati pesan pop up di Ubuntu yang seperti ini&nbsp;<b>"Ubuntu 12.04 has experienced an internal error"</b> dan kamu yakin bahwa tidak ada kesalahan pada Ubuntu yang sedang kamu gunakan. Kamu dapat menonaktifkan pelaporan Apport tersebut pada dengan trik sederhana berikut ini.<br /><center><img border="0" src="https://1.bp.blogspot.com/-bn5UsknFoog/UCziE0lJ14I/AAAAAAAACQs/eXsMuu9rf_Q/s1600/error.jpg" /></center><br />
Nah, jika kamu merasa terganggu dengan pop up seperti gambar di atas, kamu dapat membuka Terminal, kemudian mengetikkan perintah berikut:</div><pre><code>sudo gedit /etc/default/apport</code></pre><br />
Gedit Text Editor akan terbuka dan menampilkan isi "/ etc / default / profile" file.&nbsp;Yang perlu kamu lakukan di sini adalah mengubah nilai "diaktifkan" dari 1 ke 0. Setelah diubah, simpan perubahan yang kamu buat dan reboot komputermu.&nbsp;Jika kamu ingin roll semuanya kembali ke default, cukup buka lagi file tersebut dan ubah nilai "diaktifkan" ke 1.</div>
