+++
title = "NgeShare - Pasang OwnCloud 4 di Ubuntu Server 12.04"
date = 2012-08-24T05:00:00Z
tags = ["tutorial"]
comments = true
+++

<center><img border="0" data-original-height="600" data-original-width="1200" src="https://2.bp.blogspot.com/-T9DgLgimwdc/XF5OTkPsx0I/AAAAAAAATJQ/hwo3OUXxzesEtaLoyddpOZRJUYPPdxNCgCLcBGAs/s1600/owncloud.png" /></center><br />
<div style="text-align: justify;">Masih ingatkah Anda apa itu OwnCloud? <a href="http://www.owncloud.org/"><b><span style="color: #0b5394;">OwnCloud</span></b></a> merupakan salah satu aplikasi opensource yang dapat kita manfaatkan untuk melengkapi layanan Internet dasar. Tentang cloud sendiri, ada banyak definisi bisa baca. Saya menjelaskannya dari sisi aplikasi: <a href="https://www.blogger.com/blogger.g?blogID=4635419111397977465" name="more"></a>cloud adalah suatu sistem layanan di Internet yang memanfaatkan suatu server yang dikemas sedemikian hingga pengguna tidak perlu tahu lokasi fisik dan pilihan teknologi dari server yang digunakan.<br /><br />
Untuk mendapatkan layanan cloud, program aplikasi yang digunakan pengguna cukup diberitahu nama server serta protokol yang digunakannya. Kali ini OwnCloud telah mencapai versi ke-4, yang meliputi manajemen file dengan built-in file sharing ke Dropbox, streaming musik, kalender, kontak dan banyak lagi. OwnCloud versi 4  memungkinkan pengguna untuk mengembalikan versi terdahulu dari file atau melihat history file, dan penambahan penampil terintegrasi untuk file ODF.<br /><br />
Pada kesempatan ini, saya akan memberikan tips cara memasang/ menginstal OwnCloud 4 di Ubuntu server 12.04.<br /><br />
<b>Panduan Instalasi ownCloud 4 di Ubuntu Server 12,04 LTS</b><br />
Langkah 1. Untuk menginstal owncloud 4 di LTS server ubuntu 12,04, pertama install semua dependensi paket owncloud:<br />
<pre><code>sudo apt-get install apache2 php5 php5-json php-xml php-mbstring php5-zip php5-gd php5-sqlite curl libcurl3 libcurl3-dev php5-curl php-pdo</code></pre><br />
atau anda dapat menginstal <a href="http://wp.me/p26Ijz-r2">LAMP Server </a>sehingga semua dependensi paket owncloud akan secara otomatis diinstal pada server anda.<br /><br />Langkah 2. Download versi owncloud terbaru, kemudian ekstrak dan memindahkan atau menyalin ke direktori webserver /var/www:<br />
<pre><code>wget -O owncloud4.tar.bz2 http://owncloud.org/owncloud-download-4-0-0<br /><br />tar -xvf owncloud*.tar.bz2<br /><br />sudo mv owncloud /var/www/</code></pre><br />
Langkah 3. Mengatur hak akses direktori /var/www/ owncloud dengan user dan group dari pemilik webserver<br />
<pre><code>sudo chown -R www-data:www-data /var/www/owncloud<br /></code></pre><br />
Langkah 4. sekarang restart apache webserver dan mysql server<br />
<pre><code>sudo /etc/init.d/apache2 restart &amp;&amp; /etc/init.d/mysql restart</code></pre><br />
Langkah 5. Sekarang, Buka browser Anda untuk mengkonfigurasi dan menciptakan owncloud user admin.<br />
<center><img border="0" src="https://1.bp.blogspot.com/-jCafmaTh94Q/UDanOHVPkbI/AAAAAAAACa0/_-CRaLAnwc4/s1600/own1.jpg" /></center><br />
<center><img border="0" src="https://1.bp.blogspot.com/-EF4fi2IuGg4/UDanSW4kkDI/AAAAAAAACa8/_axQ69aMcY0/s1600/own2.jpg" /></center><br />
<center><img border="0" src="https://4.bp.blogspot.com/-EmQDhOlQZ4k/UDanWOGY-II/AAAAAAAACbE/-bl9GHsVcoo/s1600/own3.jpg" /></center><br />
<center><img border="0" src="https://1.bp.blogspot.com/-NTCPMeZERTc/UDanZwtfPeI/AAAAAAAACbM/lhqUZthSF2M/s1600/own4.jpg" /></center></div>
