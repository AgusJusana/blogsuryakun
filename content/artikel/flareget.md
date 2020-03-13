+++
title = "NgeShare - Install Flareget Download Manager di Ubuntu atau Linux Mint"
date = 2013-01-18T13:37:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<div style="text-align: justify;">Jika Anda seprang yang menggemari sistem operasi berbasis linux, apa yang akan Anda lakukan saat melakukan proses download file? Apakah saat melakukan hal tersebut di sistem operasi linux, Anda berandai-andai untuk memakai IDM?<br /><br />
Namun sepertinya IDM cukup sulit untuk digunakan pada sistem operasi berbasis linux. Walaupun begitu, Anda tak perlu berputus asa karena ternyata ada sebuah software mirip IDM yang dapat Anda terapkan pada Linux Anda. Software ini bernama Flareget. Software ini mempunyai fitur yang bisa dibilang hampir mirip dengan IDM, hanya saja perbedaannya terletak pada penerapan sistem operasi. Selain itu, flareget ini mempunyai sebuah keunggulan yang tak dimiliki oleh IDM (Internet Download Maneger), keuntungan tersebut ialah flareget tidak perlu menerapkan serial number pada saat proses penginstalan software ini.<br /><br />
Apakah Anda tertarik untuk mencobanya? Jika Anda ingin memasangnya pada linux Anda, saya akan memberikan panduannya berikut ini:<br /><br />
Pertama-tama, silakan unduh file<i> installer</i>-nya <a href="https://sourceforge.net/projects/flareget/" target="_blank"><b>di sini</b></a>.<br />
Setelah proses unduh selesai, instal file *.deb sesuai dengan arsitektur komputer kalian (32bit atau 64bit):<br />
<blockquote class="tr_bq">sudo dpkg - i nama-file.deb</blockquote><br />
<center><img border="0" src="https://4.bp.blogspot.com/-kKZR-c5fKbE/UPjoYysMOkI/AAAAAAAAA3w/BaC2WgdasuQ/s1600/1.png" /></center><br />
<center><img border="0" src="https://4.bp.blogspot.com/-WMarKE5k7Lk/UPjoZ7-j5AI/AAAAAAAAA30/dea_eRIR-Fs/s1600/2.png" /></center><br />
<center><img border="0" src="https://2.bp.blogspot.com/-JctES8Jwkgg/UQN0Ziti_QI/AAAAAAAABAk/upKa82vuhBs/s1600/3.png" /></center><br />
<center><img border="0" src="https://1.bp.blogspot.com/-BFnhGTAKxfI/UPjoeS-wbkI/AAAAAAAAA4E/06aT4z87nXw/s1600/4.png" /></center><br />
<center><img border="0" src="https://1.bp.blogspot.com/-e9KRkgeD_P8/UPjokbgsG0I/AAAAAAAAA4Q/I3hURrwM6XU/s1600/5.png" /></center><br />
<center><img border="0" src="https://1.bp.blogspot.com/-Dkj4TAhs6c0/UQNzzzuDAhI/AAAAAAAABAc/wywMxgckoUM/s1600/6.png" /></center><br />
<center><img border="0" src="https://1.bp.blogspot.com/-bkwyQMYIV74/UPjonPiXXvI/AAAAAAAAA4g/iAMcv4mXdDc/s1600/7.png" /></center><br />
<center><img border="0" src="https://2.bp.blogspot.com/-hh-RT674qdw/UPjosP6cbzI/AAAAAAAAA4o/SwkpLT_qrXA/s1600/flareget-ubuntu.png" /></center><br />
Anda juga dapat menginstalnya melalui PPA dengan panduan berikut ini:<br /><br />
Untuk Ubuntu / Linux Mint (32-bit), buka terminal dan masukkan perintah ini:<br /><blockquote class="tr_bq">sudo add-apt-repository ppa:upubuntu-com/flareget-i386<br />sudo apt-get update<br />sudo apt-get install flareget</blockquote><br />
Untuk sistem 64-bit, instal software dengan perintah:<br />
<blockquote class="tr_bq">sudo add-apt-repository ppa:upubuntu-com/flareget-amd64<br />sudo apt-get update<br />sudo apt-get install flareget</blockquote><br />
Jika Anda ingin menghapus software Flareget, masukkan perintah ini:<br />
<blockquote class="tr_bq">sudo add-apt-repository –remove ppa:upubuntu-com/flareget-i386</blockquote><br />
atau<br />
<blockquote class="tr_bq">sudo add-apt-repository –remove ppa:upubuntu-com/flareget-amd64<br />sudo apt-get remove flareget<br />sudo apt-get update</blockquote></div>
