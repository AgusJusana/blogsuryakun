+++
title = "NgeShare - Install PHP-Nuke 8.2 CMS di Ubuntu 12.10/12.04/Linux Mint 13"
date = 2012-11-21T14:36:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="600" data-original-width="1200" src="https://4.bp.blogspot.com/-NDkN2CeoX80/XF5Kv5fvwRI/AAAAAAAATIw/brWAepitDEIhvb_YDJf-4ym5JJeSmV_HgCLcBGAs/s1600/php.png" /></center><br />
<div style="text-align: justify;">Dalam tutorial ini, kita akan melihat bagaimana menginstal PHP Nuke 8.2 lokal dalam sistem Ubuntu/ Linux Mint. Tutorial ini juga bisa diterapkan untuk&nbsp;sistem&nbsp;lainnya yang berbasis Debian. PHP Nuke adalah CMS&nbsp;(Content Management System)&nbsp;populer yang memberikan kontrol administrator penuh atas website(portal).<br /><br />
Versi terbaru (8.2.4) datang dengan perbaikan bug lebih dan perbaikan keamanan. Anda dapat menemukan <b><a href="http://phpnuke.org/modules.php?name=Release" target="_blank"><span style="color: #0b5394;">di sini</span></a></b> fitur yang ditambahkan untuk PHP Nuke 8.2.4.<br /><br />
<b>1. Instal Server LAMP</b><br />
Untuk dapat menjalankan PHP Nuke pada sistem Anda, kita perlu menginstal terlebih dahulu web server. Untuk tutorial ini, kita akan menggunakan web server LAMP, tapi itu pilihan Anda untuk memilih web server (XAMPP misalnya). Untuk menginstal LAMP di Ubuntu 12.10/12.04/11.04 atau Linux Mint 13, buka terminal dan jalankan perintah ini:<br />
<blockquote class="tr_bq">sudo apt-get install lamp-server^</blockquote><br />
Untuk bantuan lebih lanjut tentang instalasi server LAMP, periksa <a href="http://suryapersonal.blogspot.com/2012/10/instal-lamp-server-dengan-tasksel-di.html"><b><span style="color: #0b5394;">artikel ini</span></b></a>. PHP Nuke memerlukan dukungan GD grafis. Anda dapat menginstalnya dengan perintah ini:<br />
<blockquote class="tr_bq">sudo apt-get install php5-gd</blockquote><br />
<b>2. Penurunan Dari PHP 5.4.x Untuk PHP 5.3.x</b><br />
Magic Quotes GPC telah turun dari PHP 5.4.x. Satu-satunya solusi untuk membuat PHP-Nuke bekerja di Ubuntu/ Linux Mint adalah untuk downgrade dari PHP 5.4.x ke 5.3.x. Untuk melakukan ini, Anda dapat menggunakan script sederhana yang secara otomatis akan menurunkan versi PHP Anda saat ini ke 5.3.x. Anda dapat menjalankannya dengan perintah berikut dari terminal:<br />
<blockquote>cd /tmp<br />wget http://dl.dropbox.com/u/47950494/upubuntu.com/php5_4_downgrade_5.3.sh<br />chmod +x php5_4_downgrade_5.3.sh<br />sudo sh php5_4_downgrade_5.3.sh</blockquote><br />
<b>3. Membuat Database MySQL &amp; User</b><br />
Setelah menginstal server LAMP dan menurunkan versi PHP Anda ke PHP 5.3.x, kita sekarang perlu membuat database MySQL dan user untuk digunakan dengan PHP Nuke. Jika Anda memiliki phpMyAdmin yang telah terinstal, Anda dapat dengan mudah melakukan ini dengan hanya beberapa tindakan. Tapi, jika Anda ingin membuat rincian ini dari terminal, yang menjalankan urutan perintah dan mengganti teks yang disorot dalam warna merah dengan pengaturan Anda sendiri:<br />
- Masuk ke server MySQL dengan perintah ini:<br />
<blockquote class="tr_bq">mysql -u root -p</blockquote><br />
- Buat database MySQL untuk PHP Nuke dengan perintah ini:<br />
<blockquote class="tr_bq">create database <b><span style="color: red;">phpnuke</span></b>;</blockquote><br />
- Buat user dengan perintah ini:<br />
<blockquote class="tr_bq">CREATE USER '<b><span style="color: red;">phpnuke-user</span></b>'@'localhost' IDENTIFIED BY '<b><span style="color: red;">12345</span></b>';</blockquote><br />
Ganti <b><span style="color: red;">phpnuke-user</span></b> &amp; <b><span style="color: red;">12345</span></b> dengan nama user lain dan password pilihan Anda.<br />
- Berikan akses user ke database Anda dengan perintah ini:<br />
<blockquote class="tr_bq">GRANT ALL PRIVILEGES ON <b><span style="color: red;">phpnuke</span></b>.* TO '<b><span style="color: red;">phpnuke-user</span></b>' IDENTIFIED BY '<b><span style="color: red;">12345</span></b>';</blockquote><br />
- Anda harus keluar dari server MySQL dengan perintah ini:<br />
<blockquote class="tr_bq">exit</blockquote><br />
Kami sekarang telah menciptakan rincian ini MYSQL:<br />
<ul style="text-align: justify;"><li>Hostname: <b><span style="color: red;">localhost</span></b></li><li>Database Name: <b><span style="color: red;">phpnuke</span></b></li><li>Database User: <b><span style="color: red;">phpnuke-user</span></b></li><li>Database User Password: <b><span style="color: red;">12345</span></b></li></ul><br />
<b>4. Instalasi PHP Nuke 8.2</b><br />
Anda dapat men-download dan menempatkan file PHP Nuke di <b>/var/www/</b> direktori dengan perintah:<br />
<blockquote>cd /tmp<br />sudo mkdir /var/www/phpnuke<br />wget -c http://goo.gl/iWxAv -O phpnuke-release-8.2.4.zip<br />unzip -q phpnuke-release-8.2.4.zip<br />sudo cp -r phpnuke-release-8.2.4/phpnuke/html/* /var/www/phpnuke<br />sudo chmod 777 -R /var/www/phpnuke<br />sudo /etc/init.d/apache2 restart</blockquote><br />
Kemudian Anda buka linkdi bawah ini untuk memulai instalasi PHP Nuke:<br />
<blockquote class="tr_bq"><b><span style="color: #0b5394;"><a href="http://localhost/phpnuke/install/">http://localhost/phpnuke/install/</a></span></b></blockquote><br />
<i>Catatan: Anda dapat mengganti localhost dengan alamat IP server Anda sendiri.<br /><br />
Kemudian ikuti instruksi pengaturan melalui web&nbsp;browser&nbsp;Anda.<br /><br />
Ketika Anda telah menyelesaikan proses instalasi PHP Nuke, hapus direktori install dengan perintah ini:<br />
<blockquote class="tr_bq">sudo rm -rf /var/www/phpnuke/install</blockquote></div>
