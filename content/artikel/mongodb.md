+++
title = "NgeShare - Pasang MongoDB di Ubuntu 12.04"
date = 2012-08-21T07:29:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="383" data-original-width="680" src="https://4.bp.blogspot.com/-KeCqYPbwu_I/W-1vAtoWoAI/AAAAAAAASV4/cpmy8VLPjV4Oo5eLEXmbEaN0l_eGs53ygCLcBGAs/s1600/mongodb.jpg" /></center><br />
<div style="text-align: justify;">Tutorial kami kali ini adalah tutorial&nbsp; dengan topik "Memasang <a href="https://www.mongodb.com/" target="_blank">MongoBD</a>". Ngomong-ngomong, apa itu MongoDB? MongoDB (dari "humongous") adalah sebuah open source berorientasi dokumen NoSQL Database system. MongoDB merupakan bagian dari keluarga NoSQL sistem database. Daripada menyimpan data dalam tabel seperti yang dilakukan dalam database "klasik" ​​relasional, MongoDB menyimpan data terstruktur seperti JSON-seperti dokumen dengan skema dinamis (MongoDB menyebut BSON format), membuat integrasi data dalam beberapa jenis aplikasi lebih mudah dan lebih cepat.&nbsp;MongoDB adalah database dokumen yang digunakan umumnya dalam aplikasi web modern.<br /><br />
<span style="font-size: large;"><b>Instal MongoDB di ubuntu 12.04 (Precise) Server</b></span><br />
Anda dapat memasang/ menginstal MongoBD dengan menjalankan perintah berikut ini di teminal Anda:<br />
<pre><code>sudo apt-key adv --keyserver keyserver.ubuntu.com --recv 7F0CEB10<br /><br />echo "deb http://downloads-distro.mongodb.org/repo/ubuntu-upstart dist 10gen" | tee -a /etc/apt/sources.list.d/10gen.list<br /><br />sudo apt-get -y update<br /></code></pre><br />
Jalankan perintah berikut untuk menginstal versi stabil terbaru dari MongoDB.<br />
<pre><code>sudo apt-get -y install mongodb-10gen<br /></code></pre><br /><br />
<b>Konfigurasi MongoDB</b><br />
Paket-paket mengkonfigurasi MongoDB menggunakan file / etc / mongodb.conf dalam hubungannya dengan script kontrol. Untuk sistem berbasis Upstart, menemukan script kontrol di / etc / init / mongodb.conf.<br /><br />
Ini contoh MongoDB akan menyimpan file data dalam / var / lib / mongodb dan yang log file dalam / var / log / mongodb, dan menjalankan menggunakan account pengguna mongodb.<br /><br />
<span style="font-size: large;"><b>Mengontrol MongoDB</b></span><br />
<b>Mulai MongoDB</b><br />
Pengguna pemula dapat memulai proses mongod dengan mengeluarkan perintah berikut:<br />
<pre><code>sudo service mongodb start<br /></code></pre><br />
<b>Menghentikan MongoDB</b><br />
Pengguna pemula dapat menghentikan proses mongod dengan mengeluarkan perintah berikut:<br />
<pre><code>sudo service mongodb stop<br /></code></pre><br />
Pengguna pemula dapat memulai proses mongod dengan mengeluarkan perintah berikut:<br />
<pre><code>sudo service mongodb restart<br /></code></pre><br />
<b>Mengontrol Mongos</b><br />
Pada rilis saat ini, tidak ada skrip kontrol untuk Mongos. Mongos hanya digunakan dalam sharding penyebaran dan biasanya tidak berjalan pada sistem yang sama di mana mongod berjalan. Anda dapat menggunakan script mongodb direferensikan di atas untuk mendapatkan script sendiri Mongos kontrol.<br />
<b>Menggunakan MongoDB</b><br />
Di antara alat-alat disertakan dengan paket MongoDB, adalah shell mongo. Anda dapat terhubung ke instance MongoDB Anda dengan mengeluarkan perintah berikut pada sistem prompt:<br />
<pre><code>mongo<br /></code></pre><br />
Ini akan terhubung ke database berjalan pada interface localhost secara default. Pada prompt mongo, mengeluarkan dua perintah berikut untuk memasukkan catatan dalam koleksi "test" dari database (default) "test".<br />
<pre><code>&gt; db.test.save( { a: 1 } )<br /><br />&gt; db.test.find()<br /></code></pre></div>
