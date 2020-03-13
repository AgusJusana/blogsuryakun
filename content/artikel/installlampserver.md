+++
title = "NgeShare - Install Lamp Server dengan Tasksel di Ubuntu 12.10/12.04 dan Linux Mint 13"
date = 2012-10-09T13:31:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="600" data-original-width="1200" src="https://2.bp.blogspot.com/-MrzG1b8XjQk/XF5LaW5u5tI/AAAAAAAATI4/B2SI0dzujRUbX0jIKf2iygOmoCOx9pu2wCLcBGAs/s1600/lamp.png" /></center><br />
<div style="text-align: justify;">Salam linuxer! Oke kali ini saya akan membagikan sebuah tutorial yaitu tutorial cara menginstal Lamp Server dengan menggunakan Tasksel. Sebelumnya apa itu Lamp Server?<br />
<center><img border="0" data-original-height="432" data-original-width="800" src="https://1.bp.blogspot.com/-li9Ynnprphk/W-6qCGhMeDI/AAAAAAAASZo/TJ5nV_3AakwBhs_IEb6AzGfv5V9xanbcwCLcBGAs/s1600/lamp_stack.jpg" /></center><br />
Lamp Server adalah singkatan dari Linux, Apache, MySQL dan PHP adalah sebuah set instalasi yang sangat populer untuk sebuah web server yang mendukung PHP dan MySQL.<br /><br />
Tutorial ini dapat Anda coba pada Ubuntu 12.10/12.04 atau di Linux Mint 13 milik Anda.<br /><br />
<b>Instal Lamp Server</b><br />
Buka terminal dan install terlebih dahulu tasksel dengan perintah ini:<br />
<pre><code>sudo apt-get -y install tasksel<br /></code></pre><br />
Mulai sekarang tasksel dengan perintah ini:<br />
<pre><code>sudo tasksel<br /></code></pre><br />
Pilih "LAMP&nbsp;server" dari daftar yang diberikan menggunakan spasi dan tekan Enter:<br />
<center><img border="0" src="https://1.bp.blogspot.com/-YS0WxnpjWHE/UHPB9tV8zxI/AAAAAAAAEUM/UPdqEPDoKQ8/s1600/Ubuntu-lamp2.jpg" /></center><br />
Setelah Anda menyelesaikan instalasi LAMP&nbsp;server, periksa apakah itu bekerja dengan membuka salah satu link (menggunakan IP&nbsp;server&nbsp;jika diperlukan):<br />
<pre><code>http://localhost/</code></pre><br />
atau dengan menggunakan:<br />
<pre><code>http://127.0.0.1/<br /></code></pre><br />
Anda harus melihat halaman ini:<br />
<center><img border="0" src="https://3.bp.blogspot.com/-GKdKA3x4yK4/UHPCtogNHDI/AAAAAAAAEUU/tJeM4ZbfR9Y/s1600/ubuntu-lamp3.png" /></center><br />
Jika tidak muncul, cobalah untuk me-restart Apache dengan perintah ini:<br />
<pre><code>sudo /etc/init.d/apache2 restart</code></pre><br />
Anda juga dapat menginstal LAMP&nbsp;server&nbsp;dengan perintah ini:<br />
<pre><code>sudo tasksel install lamp-server<br /></code></pre><br />
Untuk menguji apakah PHP terpasang dengan baik, jalankan perintah ini:<br />
<pre><code>echo "" | sudo tee /var/www/test.php<br /><br />sudo /etc/init.d/apache2 restart</code></pre><br />
Kemudian buka link ini:<br />
<pre><code>http://localhost/test.php</code></pre><br />
File PHP Anda dan proyek harus ditempatkan dalam folder ini:<br />
<pre><code>/var/www/</code></pre><br />
Anda dapat mengaksesnya dengan hak akses root menggunakan perintah ini:<br />
<pre><code>sudo nautilus /var/www/ <br /></code></pre></div>
