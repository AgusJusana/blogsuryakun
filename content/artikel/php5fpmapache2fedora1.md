+++
title = "NgeShare - Mencoba PHP5-FPM Dengan Apache2 di Fedora 17 Part 1"
date = 2012-09-18T17:59:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="350" data-original-width="722" src="https://1.bp.blogspot.com/-bj6zNfLNra4/W-4gk938VYI/AAAAAAAASYs/MhC3-pi4AZg7Qf1LiyQ_RBz8IvlnOSSFACLcBGAs/s1600/php.jpg" /></center><br />
<div style="text-align: justify;">Tutorial ini menunjukkan bagaimana Anda dapat memasang webserver Apache2 pada server Fedora 17 dengan PHP5 (melalui PHP-FPM) dan dukungan MySQL. PHP-FPM (FastCGI Process Manager) merupakan alternatif PHP FastCGI implementasi dengan beberapa fitur tambahan yang berguna untuk situs dari berbagai ukuran, terutama situs sibuk. Saya tidak mengeluarkan jaminan bahwa ini akan bekerja untuk Anda!<br /><br />
<b>1. Pendahuluan Catatan</b><br />
Dalam tutorial ini saya menggunakan server1.example.com nama host dengan alamat IP 192.168.0.100. Pengaturan ini mungkin berbeda untuk Anda, jadi Anda harus mengganti mereka di mana perlu.<br /><br />
<b>2. Tambahan Repositori Mengaktifkan</b><br />
Kita perlu menginstal mod_fastcgi nanti yang tersedia di repositori rpmforge. Rpmforge bisa difungsikan sebagai berikut:<br />
<pre><code>rpm --import http://dag.wieers.com/rpm/packages/RPM-GPG-KEY.dag.txt<br /><br />cd /tmp<br /><br />wget http://pkgs.repoforge.org/rpmforge-release/rpmforge-release-0.5.2-2.el6.rf.x86_64.rpm<br /><br />rpm -ivh rpmforge-release-0.5.2-2.el6.rf.x86_64.rpm<br /></code></pre><br />
<b>3. Instalasi MySQL 5</b><br />
Untuk menginstal MySQL, kita melakukan ini:<br />
<pre><code>yum install mysql mysql-server<br /></code></pre><br />
Kemudian kita membuat link startup sistem untuk MySQL (sehingga MySQL dijalankan secara otomatis setiap kali sistem boot) dan memulai server MySQL:<br />
<pre><code>systemctl enable mysqld.service<br /><br />systemctl start mysqld.service<br /></code></pre><br />
Set password untuk akun root MySQL:<br />
<pre><code>mysql_secure_installation<br /></code></pre><br />
<b>4. Instalasi Apache2</b><br />
Apache2 tersedia sebagai paket Fedora, oleh karena itu kita dapat menginstalnya seperti ini:<br />
<pre><code>yum install httpd<br /></code></pre><br />
Sekarang mengkonfigurasi sistem anda untuk memulai Apache pada saat boot ...<br />
<pre><code>systemctl enable httpd.service<br /></code></pre><br />
... dan mulai Apache:<br />
<pre><code>systemctl start httpd.service<br /></code></pre><br />
Sekarang langsung browser Anda untuk http://192.168.0.100, dan anda akan melihat halaman placeholder Apache2:<br />
<center><img border="0" src="https://2.bp.blogspot.com/-VUbH7PrbyBo/UFhR2CeU_HI/AAAAAAAADSM/jMDaYlZXlvo/s1600/1.png" /></center><br />
Standar akar dokumen Apache adalah / var / www / html pada Fedora, dan file konfigurasi / etc / httpd / conf / httpd.conf. Konfigurasi tambahan disimpan di direktori / etc / httpd / conf.d /.<br /><br />
<b>5. Instalasi PHP5</b><br />
Kita bisa membuat PHP5 bekerja di Apache2 melalui PHP-FPM dan modul mod_fastcgi Apache yang kita install sebagai berikut:<br />
<pre><code>yum install mod_fastcgi php-fpm<br /></code></pre><br />
Kemudian buka / etc / php.ini:<br />
<pre><code>vi /etc/php.ini<br /></code></pre><br />
Untuk menghindari kesalahan seperti:<br />
<pre><code>[08-Aug-2011 18:07:08] PHP Warning: phpinfo(): It is not safe to rely on the system's timezone settings. You are *required* to use the date.timezone setting or the date_default_timezone_set() function. In case you used any of those methods and you are still getting this warning, you most likely misspelled the timezone identifier. We selected 'Europe/Berlin' for 'CEST/2.0/DST' instead in /usr/share/nginx/html/info.php on line 2<br /><br />... in /var/log/php-fpm/www-error.log when you call a PHP script in your browser, you should set date.timezone in /etc/php.ini<br /><br />[...]<br />[Date]<br />; Defines the default timezone used by the date functions<br />; http://php.net/date.timezone<br />date.timezone = "Europe/Berlin"<br />[...]<br /></code></pre><br />
Anda dapat mengetahui zona waktu yang benar untuk sistem Anda dengan menjalankan:<br />
<pre><code>cat /etc/sysconfig/clock<br /></code></pre><br />
Selanjutnya menciptakan sistem link startup untuk php-fpm dan memulainya:<br />
<pre><code>systemctl enable php-fpm.service<br /><br />systemctl start php-fpm.service<br /></code></pre><br />
PHP-FPM adalah proses daemon (dengan script / etc init / init.d / php-fpm) yang menjalankan server FastCGI pada port 9000.<br /><br />
Selanjutnya me-restart Apache:<br />
<pre><code><br />systemctl restart httpd.service<br /></code></pre></div>
