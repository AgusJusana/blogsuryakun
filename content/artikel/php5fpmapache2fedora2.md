+++
title = "NgeShare - Mencoba PHP5-FPM Dengan Apache2 di Fedora 17 Part 2"
date = 2012-09-18T18:33:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="350" data-original-width="722" src="https://1.bp.blogspot.com/-bj6zNfLNra4/W-4gk938VYI/AAAAAAAASYs/MhC3-pi4AZg7Qf1LiyQ_RBz8IvlnOSSFACLcBGAs/s1600/php.jpg" /></center><br />
<div style="text-align: justify;">Berikut ini adalah postingan lanjutan dari postingan kami yang berjudul <b>"Menjajal PHP5-FPM Dengan Apache2 di Fedora 17 Part 1"</b>. Mari kita simak lanjutannya.<br /><br />
<b>6. Konfigurasi Apache</b><br />
Untuk membuat Apache bekerja sama dengan PHP-FPM, kita perlu konfigurasi sebagai berikut:<br />
<pre><code><ifmodule mod_fastcgi.c="">&lt;IfModule mod_fastcgi.c&gt;</ifmodule></code></pre><pre><code><ifmodule mod_fastcgi.c="">     DirectoryIndex index.html index.shtml index.cgi index.php</ifmodule></code></pre><pre><code><ifmodule mod_fastcgi.c="">     AddHandler php5-fcgi .php</ifmodule></code></pre><pre><code><ifmodule mod_fastcgi.c="">     Action php5-fcgi /php5-fcgi</ifmodule></code></pre><pre><code><ifmodule mod_fastcgi.c="">     Alias /php5-fcgi /usr/lib/cgi-bin/php5-fcgi</ifmodule></code></pre><pre><code><ifmodule mod_fastcgi.c="">     FastCgiExternalServer /usr/lib/cgi-bin/php5-fcgi -host 127.0.0.1:9000 -pass-header Authorization<br />&lt;/IfModule&gt;</ifmodule><br /></code></pre><br />
(Untuk mempelajari lebih lanjut tentang direktif FastCgiExternalServer, lihatlah <a href="http://www.fastcgi.com/mod_fastcgi/docs/mod_fastcgi.html">http://www.fastcgi.com/mod_fastcgi/docs/mod_fastcgi.html</a> #FastCgiExternalServer.)<br /><br />Anda dapat memasukkannya ke dalam konfigurasi Apache global (sehingga itu diaktifkan untuk semua vhosts), misalnya di / etc / httpd / conf.d / fastcgi.conf, atau Anda bisa menempatkannya di setiap vhost yang harus menggunakan PHP-FPM. Saya ingin menggunakan PHP-FPM dengan semua vhosts jadi saya membuka / etc / httpd / conf.d / fastcgi.conf ...<br />
<pre><code>vi /etc/httpd/conf.d/fastcgi.conf</code></pre><br />
... dan menempatkan bagian berikut di akhir:<code></code><br />
<pre><code>[...]<br />        &lt;IfModule mod_fastcgi.c&gt;<br />                DirectoryIndex index.html index.shtml index.cgi index.php<br />                AddHandler php5-fcgi .php<br />                Action php5-fcgi /php5-fcgi<br />                Alias /php5-fcgi /usr/lib/cgi-bin/php5-fcgi<br />                FastCgiExternalServer /usr/lib/cgi-bin/php5-fcgi -host 127.0.0.1:9000 -pass-header Authorization<br />        &lt;/IfModule&gt;<ifmodule mod_fastcgi.c="">   </ifmodule></code></pre><br />
The / usr / lib / cgi-bin / direktori harus ada, jadi kami menciptakannya sebagai berikut:<br />
<pre><code>mkdir /usr/lib/cgi-bin/</code></pre><br />
Jika mod_php terinstal dan diaktifkan, kita perlu menonaktifkannya. Buka file / etc / httpd / conf.d / php.conf ...<br />
<pre><code>vi /etc/httpd/conf.d/php.conf</code></pre><br />
... dan komentar pada AddHandler dan garis AddType:<br />
<pre><code>#<br /># PHP is an HTML-embedded scripting language which attempts to make it<br /># easy for developers to write dynamically generated webpages.<br />#<br />&lt;IfModule prefork.c&gt;<br />  LoadModule php5_module modules/libphp5.so<br />&lt;/IfModule&gt;<br />&lt;IfModule !prefork.c&gt;<br />  LoadModule php5_module modules/libphp5-zts.so<br />&lt;/IfModule&gt;<br /><br /><br />#<br /># Cause the PHP interpreter to handle files with a .php extension.<br />#<br />#AddHandler php5-script .php<br />#AddType text/html .php<br /><br />#<br /># Add index.php to the list of files that will be served as directory<br /># indexes.<br />#<br />DirectoryIndex index.php<br /><br />#<br /># Uncomment the following line to allow PHP to pretty-print .phps<br /># files as PHP source code:<br />#<br />#AddType application/x-httpd-php-source .phps<br /></code></pre><br />
Restart Apache setelah:<br />
<pre><code>systemctl restart httpd.service<br /></code></pre><br />
Sekarang membuat file PHP berikut dalam document root / var / www / html dari default Apache vhost:<code></code><br /><pre><code>vi /var/www/html/info.php</code></pre><br />
<table bgcolor="#CCCCCC" border="1" bordercolor="#000000" cellpadding="2" cellspacing="0" class="" style="background-color: white; border-collapse: collapse; border: 1px solid rgb(255, 255, 255); color: black; font-family: &quot;verdana&quot;, sans-serif; font-size: 12px; line-height: 18px; margin: 0px 0px 1em; padding: 0px; text-align: left; width: 90%;"><tbody style="margin: 0px; padding: 0px;"><tr style="margin: 0px; padding: 0px;"><td class="" style="font-size: 11px; margin: 0px; padding: 2px; vertical-align: top;"><pre style="background-color: #efefef; border: 1px inset; font-size: 16px; height: 250px; overflow: auto; padding: 6px; width: 500px;">&lt;?php<br />phpinfo();<br />?&gt;</pre></td></tr></tbody></table><br />
Sekarang kita sebut file tersebut dalam browser (misalnya http://192.168.0.100/info.php):<br />
<center><img border="0" src="https://2.bp.blogspot.com/-3mgb6ipHiME/UFhYsM6XPBI/AAAAAAAADTQ/fVNLNf_JFT0/s1600/2.png" /></center><br />
Seperti yang Anda lihat, PHP5 bekerja, dan itu bekerja melalui FPM / FastCGI, seperti yang ditunjukkan pada baris Server API. Jika Anda menggulir ke bawah, Anda akan melihat semua modul yang sudah diaktifkan di PHP5. MySQL tidak terdaftar di sana yang berarti kita tidak memiliki dukungan MySQL di PHP5 belum.<br /><b><br />7. Mendapatkan Dukungan MySQL Pada PHP5</b><br />Untuk mendapatkan dukungan MySQL di PHP, kita dapat menginstal paket php-mysql. Ini adalah ide yang baik untuk menginstal beberapa modul PHP5 lainnya serta Anda mungkin membutuhkannya untuk aplikasi Anda. Anda dapat mencari PHP5 tersedia modul seperti ini:<br />
<pre><code>yum search php</code></pre><br />
Pilih yang Anda butuhkan dan menginstalnya seperti ini:<br />
<pre><code>yum install php-mysql php-gd php-imap php-ldap php-odbc php-pear php-xml php-xmlrpc php-magickwand php-mbstring php-mcrypt php-mssql php-shout php-snmp php-soap php-tidy</code></pre><br />
APC adalah PHP bebas dan terbuka opcode cacher untuk caching dan mengoptimalkan kode menengah PHP. Ini mirip dengan opcode cachers lain PHP, seperti eAccelerator dan XCache. Hal ini sangat dianjurkan untuk memiliki salah satu diinstal untuk mempercepat halaman PHP Anda.<br /><br />
APC dapat diinstal sebagai berikut:<br />
<pre><code>yum install php-pecl-apc<br /></code></pre><br />
Sekarang muat ulang PHP-FPM:<br />
<pre><code>systemctl reload php-fpm.service<br /></code></pre><br />
Sekarang muat ulang http://192.168.0.100/info.php di browser Anda dan gulir ke bawah ke bagian modul lagi. Anda sekarang harus menemukan banyak modul baru di sana, termasuk modul MySQL.<br /><br />
<b>8. phpMyAdmin</b><br />
phpMyAdmin adalah antarmuka web di mana Anda dapat mengelola database MySQL. Ini adalah ide yang baik untuk menginstalnya:<br />
<pre><code>yum install phpmyadmin<br /></code></pre><br />
Sekarang kita mengkonfigurasi phpMyAdmin. Kami mengubah konfigurasi Apache sehingga phpMyAdmin yang memungkinkan koneksi tidak hanya dari localhost (dengan komentar dari "/usr/share/phpmyadmin"&gt; bait &lt;Directory):<br />
<pre><code>vi /etc/httpd/conf.d/phpmyadmin.conf<br /></code></pre><br />
<table bgcolor="#CCCCCC" border="1" bordercolor="#000000" cellpadding="2" cellspacing="0" class="" style="background-color: white; border-collapse: collapse; border: 1px solid rgb(255, 255, 255); color: black; font-family: &quot;verdana&quot;, sans-serif; font-size: 12px; line-height: 18px; margin: 0px 0px 1em; padding: 0px; text-align: left; width: 90%;"><tbody style="margin: 0px; padding: 0px;"><tr style="margin: 0px; padding: 0px;"><td class="" style="font-size: 11px; margin: 0px; padding: 2px; vertical-align: top;"><pre style="background-color: #efefef; border: 1px inset; font-size: 16px; height: 250px; overflow: auto; padding: 6px; width: 500px;">#<br />#  Web application to manage MySQL<br />#<br /><br />#&lt;Directory "/usr/share/phpmyadmin"&gt;<br />#  Order Deny,Allow<br />#  Deny from all<br />#  Allow from 127.0.0.1<br />#&lt;/Directory&gt;<br /><br />Alias /phpmyadmin /usr/share/phpmyadmin<br />Alias /phpMyAdmin /usr/share/phpmyadmin<br />Alias /mysqladmin /usr/share/phpmyadmin</pre></td></tr></tbody></table><br />
Selanjutnya kita mengubah otentikasi di phpMyAdmin dari cookie ke http:<br />
<pre><code>vi /usr/share/phpmyadmin/config.inc.php<br /></code></pre><br />
<table bgcolor="#CCCCCC" border="1" bordercolor="#000000" cellpadding="2" cellspacing="0" class="" style="background-color: white; border-collapse: collapse; border: 1px solid rgb(255, 255, 255); color: black; font-family: &quot;verdana&quot;, sans-serif; font-size: 12px; line-height: 18px; margin: 0px 0px 1em; padding: 0px; text-align: left; width: 90%;"><tbody style="margin: 0px; padding: 0px;"><tr style="margin: 0px; padding: 0px;"><td class="" style="font-size: 11px; margin: 0px; padding: 2px; vertical-align: top;"><pre style="background-color: #efefef; border: 1px inset; font-size: 16px; height: 250px; overflow: auto; padding: 6px; width: 500px;">[...]<br />/* Authentication type */<br />$cfg['Servers'][$i]['auth_type'] = 'http';<br />[...]</pre></td></tr></tbody></table><<br />
Restart Apache:<br />
<pre><code>systemctl restart httpd.service<br /></code></pre><br />
Setelah itu, Anda dapat mengakses phpMyAdmin di bawah http://192.168.0.100/phpmyadmin/:<br />
<center><img border="0" src="https://3.bp.blogspot.com/-_C9W7u9IwQI/UFhbCcw5N6I/AAAAAAAADTY/AncSKmGQwmM/s1600/4.png" /></center></div>
