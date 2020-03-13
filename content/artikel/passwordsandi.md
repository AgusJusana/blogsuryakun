+++
title = "NgeShare - Cara Melindungi File atau Folder di Ubuntu / Linux Mint dengan Password/ Sandi"
date = 2013-01-08T03:25:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="512" data-original-width="512" height="200" src="https://2.bp.blogspot.com/-cZC-u3Fgn60/W--RqkabNQI/AAAAAAAASdM/rhwkmxXmN74-bSwbVBja_253gt6mnWg_gCLcBGAs/s200/security.jpg" width="200" /></center><br />
<div style="text-align: justify;">Dalam tutorial ini, saya akan menjelaskan cara mudah melindungi file atau folder di Ubuntu / Linux Mint dengan password/ sandi. Anda tidak harus menggunakan perangkat lunak pihak ketiga, kita hanya akan menggunakan manajer arsip untuk kompres file atau folder dan menguncinya dengan password sehingga pengguna komputer yang tidak sah tidak dapat menyalin file atau folder Anda tersebut.<br /<br />
Pertama yang harus Anda lakukan adalah&nbsp;Klik kanan pada file atau folder dan pilih Compress:<br />
<center><img border="0" src="https://3.bp.blogspot.com/-j4Y0j1Ks_TA/UOst6M36kYI/AAAAAAAAAx0/hCsfZZ8vHpc/s1600/pass-protect-1.png" /></center><br />
Pada jendela yang akan muncul, pilih compression format (7z, zip, tar, dll), kemudian klik Other Options:<br /
<center><img border="0" src="https://3.bp.blogspot.com/-qp0dmGYSCtI/UOsuEqjKV5I/AAAAAAAAAx8/ZMZhDPfNnxI/s1600/pass-protect-2.png" /></center><br />
Masukkan password yang Anda inginkan, centang "Encrypt the file list too", kemudian klik Create:<br />
<center><img border="0" src="https://1.bp.blogspot.com/-LlhaSGS5MyU/UOsuQwWlkQI/AAAAAAAAAyE/lYXrTAfZayE/s1600/pass-protect-3.png" /></center><br />
File/ folder Anda sekarang yang telah dikompres telah terlidungi oleh password/ sandi. Pengguna lain dapat mengekstrak file/ folder Anda asalkan mereka mengetahui/ memberian password yang benar.<br />
<center><img border="0" src="https://1.bp.blogspot.com/-8LxkgsoxCQA/UOsuYqIh2eI/AAAAAAAAAyM/ypS7oM9xyos/s1600/pass-protect-4.png" /></center><br />
Jika Anda ingin mencegah pengguna lain menghapus atau memindahkan file yang dilindungi password/ sandi yang baru Anda buat, buka terminal dan cd ke tempat file/ folder itu disimpan, kemudian jalankan perintah ini:<br />
<blockquote class="tr_bq">sudo  chattr +i file-name.ext</blockquote><br />
Untuk membatalkan, masukkan perintah ini:<br />
<blockquote class="tr_bq">sudo  chattr -i file-name.ext </blockquote></div>
