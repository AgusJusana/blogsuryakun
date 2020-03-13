+++
title = "NgeShare - Cara Mengubah Splash Screen LibreOffice 3.6.x di Ubuntu/ Linux Miint"
date = 2012-11-12T05:09:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="600" data-original-width="1200" src="https://3.bp.blogspot.com/-D8EsuBQ_y0g/XNIqcem74lI/AAAAAAAATkI/qcq-Usn96XoIYXFWo1Fz6ypriRLKo584QCLcBGAs/s1600/libre.png" /></center><br />
<div style="text-align: justify">Dalam tutorial ini, kita akan melihat bagaimana mengubah splash screen LibreOffice 3.6.x di Ubuntu/ Linux Mint. Jika Anda belum membuat splash screen Anda sendiri, Anda dapat mencari dan mengunduh beberapa dari mereka <b><a href="https://www.gnome-look.org/" target="_blank"><span style="color: #0b5394;">di sini</span></a></b>.<br />
<center><img border="0" src="https://1.bp.blogspot.com/-5A7FKZqZKIw/UKAgTXjr1QI/AAAAAAAAADg/ZHfWNmWJxxc/s1600/libreoffice-splash-screen-default.png" /></center><br />
<center><img border="0" src="https://3.bp.blogspot.com/-ATAtZAIIAL8/UKAgPQekJOI/AAAAAAAAADY/nxEeXomh_fA/s1600/libreoffice-splash-screen-blue.png" /></center><br />
<center><img border="0" src="https://4.bp.blogspot.com/-jze9hwokPTk/UKAgYKPvQbI/AAAAAAAAADo/doZ39C2YOJ0/s1600/libreoffice-splash-screen-mix.png" /></center><br />
<b><span style="font-size: large;">Instal Libre Office 3.6.x</span></b><br />
Jika Anda belum upgrade ke LibreOffice 3.6, kemudian melakukan dengan perintah di bawah Ubuntu 12.10/12.04/Linux Mint 13:<br />
<blockquote>sudo apt-get purge libreoffice-core<br />sudo add-apt-repository ppa:libreoffice/libreoffice-prereleases<br />sudo apt-get update<br />sudo apt-get install libreoffice</blockquote><br />
<b><span style="font-size: large;">Mengubah&nbsp;Splash Screen&nbsp;LibreOffice 3.6.x</span></b><br />
Mari kita backup pertama layar default percikan hijau dengan perintah ini:<br />
<blockquote class="tr_bq">sudo mv /usr/lib/libreoffice/program/intro.png /usr/lib/libreoffice/program/intro.png.back</blockquote><br />
Sekarang mengubah nama splash screen kustom Anda untuk intro.png dan memindahkannya dengan perintah ini:<br />
<blockquote class="tr_bq">sudo mv intro.png /usr/lib/libreoffice/program/</blockquote><br />
Untuk mengembalikan splash screen default, jalankan perintah ini:<br />
<blockquote class="tr_bq">sudo mv /usr/lib/libreoffice/program/intro.png.back /usr/lib/libreoffice/program/intro.png</blockquote><br />
<b><i>Note: </i></b><i>Tips ini juga bisa diterapkan untuk LibreOffice 3.5.x.</i></div>
