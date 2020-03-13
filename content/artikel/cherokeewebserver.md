+++
title = "NgeShare - Install Cherokee Webserver di Ubuntu 13.04"
date = 2013-09-07T17:38:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" src="https://3.bp.blogspot.com/-HlVPriAelBs/UisB74m20RI/AAAAAAAADCE/KUrm-MSXnp0/s1600/Cherokee.png" /></center><br />
<div style="text-align: justify;">Kali ini ane mau bagi-bagi tutorial cara menginstall Cherokee webserver di Ubuntu 13.04. Sekiranya tutorial ini dapat membantu bagi agan-agan yang punya proyek yang berkaitan dengan webserver. Sebelum memulai tutorial ini, apa sih Cherokee itu gan?<br /><br />
Cherokee adalah sebuah webserver dengan kinerja yang tinggi. Sangat cepat, fleksibel dan mudah dikonfigurasi gan. Menawarkan dukungan untuk widespread teknologi saat ini. Selain itu, Cherokee sangat efisien, ringan dan memberikan stabilitas rock yang solid. Di antara banyak fitur-fitur dalam Cherokee, terdapat satu fitur yang special untuk kita apresiasikan. Fitur ini bernama Cherokee-Admin yang disediakan untuk mempermudah agan dalam pengkonfigurasian setiap fitur tunggal di server.<br /><br />
Gimana udah tau sekilas kan tentang Cherokee webserver? Kalau agan pengen tau lebih lengkapnya mengenai Cherokee webserver, coba aja silahturahmi ke web resminya <a href="http://cherokee-project.com/"><b>di sini</b></a> atau install aja di Ubuntu agan dengan mengikuti tutorial ane di bawah ini. Yuk mari, hehehe....<br />
1. Masukkan perintah di bawah ini ke dalam terminal:<br />
<blockquote class="tr_bq">sudo apt-get install python-software-properties</blockquote><br />
2. Tambahkan Cherokee webserver dengan perintah ini:<br />
<blockquote class="tr_bq">sudo add-apt-repository ppa:cherokee-webserver</blockquote><br />
3. Update source list<br />
<blockquote class="tr_bq">sudo apt-get update </blockquote><br />
4. Berikut perintah Cherokee webserver, Cherokee GUI admin interface, modul SSL untuk Cherokee:<br />
<blockquote class="tr_bq">sudo apt-get install cherokee libcherokee-mod-libssl libcherokee-mod-streaming libcherokee-mod-rrd </blockquote><br />
5. Sekarang agan mulai Cherokee webserver admin interface menggunakan perintah di bawah ini. Jika agan tidak menggunakan opsi-b secara default, cherokee-admin hanya dapat mengakses dari localhost. Jika agan tidak menyebutkan alamat ip, maka secara otomatis akan mendengarkan semua interface jaringan. Kemudian agan dapat terhubung ke cherokee-admin dari alamat jaringan lainnya.<br />
<blockquote class="tr_bq">sudo cherokee-admin -b</blockquote><br />
Akan muncul tampilan seperti berikut:<br />
<pre><code class="language-markup">Cherokee Web Server 1.2.101 (Apr 29 2013): Listening on port ALL:9090, TLS disabled, IPv6 enabled, using epoll, 4096 fds system limit, max. 2041 connections, caching I/O, single thread<br />Login:<br />User: admin<br />One-time Password: k2qRxxxxxxxxxxxx (password berbeda/ menyesuaikan)<br />Web Interface:<br />URL: http://localhost:9090/</code></pre><br />
Sekarang agan dapat mengakses panel administrasi Cherokee dari browser favorit agan dengan mengetikkan url http://hostname_or_IP:9090/<br />
<center><img border="0" src="https://4.bp.blogspot.com/-35zvu1RGp3Y/UisBW9ScQ4I/AAAAAAAADB8/YFyNujs7nxQ/s1600/cherokee_preview.png" /></center><br />
Agan dapat mengakses cherokee admin dari alamat jaringan tertentu menggunakan perintah berikut:<br />
<pre><code class="language-markup">sudo cherokee-admin -b 192.168.56.10</code></pre></div>
