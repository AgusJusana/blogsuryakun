+++
title = "NgeShare - Install Oracle Java Secara Manual di Ubuntu"
date = 2012-09-29T16:18:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="968" data-original-width="1600" src="https://3.bp.blogspot.com/-LJ4Z7lyS1Gs/W-6Bs_UrggI/AAAAAAAASZQ/X7KJ4KcVIHgRwe6N1zaFD2evuwigvIFCgCLcBGAs/s1600/oracle_java.jpg" /></center><br />
<div style="text-align: justify;">Nah, sudah ada PPA yang berisi script instalasi Oracle Java di Ubuntu. Script ini secara otomatis men-download installer dari situs Oracle, menginstalnya pada komputer, dan akhirnya mengkonfigurasi sebagai default JVM pada Ubuntu.<br /><br />
Menggunakan script installer adalah cara termudah untuk menyelesaikan sesuatu, tetapi dalam kasus Anda tidak percaya script yang dapat merusak sistem Anda, Anda masih dapat menginstal Oracle Java secara manual. Anda melakukan semua hal ini sendiri.<br /><br />
<b>Mendownload biner</b><br />
Hal pertama yang pertama, silahkan download biner Oracle Java dari <b><a href="http://www.oracle.com/technetwork/java/javase/downloads/index.html">website Oracle</a></b>. Jika Anda ingin mengembangkan aplikasi Java, Anda harus memilih JDK, tetapi jika Anda ingin hanya menjalankan aplikasi Java, JRE harus cocok untuk Anda.<br /><br />
Setelah tombol download diklik, Anda akan ditawarkan dengan banyak pilihan download. Silahkan download versi yang sesuai untuk arsitektur sistem Anda, dan pastikan Anda memilih file yang memiliki *. Tar.gz ekstensi.<br /><br />
<b>Instalasi di Ubuntu</b><br />
Setelah file biner download, jalankan perintah berikut untuk menginstal Oracle Java di Ubuntu:<br />
<pre><code>sudo tar -zxvf jdk-7u7-linux-i586.tar.gz -C /usr/lib/jvm/</code></pre><br />
<b>Konfigurasi Java default di Ubuntu</b><br />
Setelah Oracle Java diinstal, Anda perlu memberitahu sistem bahwa Anda baru saja menginstal Java baru, dan secara opsional menjadikannya sebagai default JVM di Ubuntu:<br />
<pre><code>for alt in java javac; do sudo update-alternatives --install /usr/bin/$alt $alt /usr/lib/jvm/jdk*/bin/$alt 1000; done</code></pre><br />
Opsional, jalankan perintah berikut untuk memilih Java default pada Ubuntu:<br />
<pre><code>for alt in java javac; do sudo update-alternatives --config $alt; done</code></pre><br />
Periksa apakah Java Oracle ditetapkan sebagai standar Java dengan mengetikkan:<br />
<pre><code>java -version<br /></code></pre><br />
<center><img border="0" src="https://3.bp.blogspot.com/-Xb43E8C7Ro8/UGa8Jgph1yI/AAAAAAAAD7I/i1okLjLjL00/s1600/Selection_491.png" /></center></div>
