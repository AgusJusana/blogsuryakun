+++
title = "NgeShare - Cara Menginstal Remastersys di Ubuntu 12.04"
date = 2012-08-02T14:14:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<div style="text-align: justify;">Bagi agan-agan yang lagi giat-giatnya berkecimpung di dunia linux dan sedang punya proyek remaster linux khususnya me<i>remaster</i> linux Ubuntu, saya punya alternatif agar proyek agan tersebut berhasil alias succes. Saya sendiri di sini juga sedang dihadapan pada sebuah proyek remaster, saya menggunakan sebuah software yang bernama Remastersys. Saya akan memberikan info tentang cara menginstal software ini, kalau agan-agan mau instal juga, bisa dilihat caranya di bawah ini.<br />
<center><img border="0" src="https://2.bp.blogspot.com/-BhS4pixOkYg/UBoowBMO40I/AAAAAAAACCU/a39_lJJytOI/s1600/remastersys.jpg" /></center><br />
Cara install remastersys pada ubuntu 12.04:<br />
1. Agan buka terminal atau ctrl+alt+t.
2. Ketik command :<br />
<pre><code>sudo su</code></pre><br />
Kemudian masukkan password Agan.<br />
3. masih sama di terminal/root ketikkan command:<br />
<pre><code>wget -O – http://www.remastersys.com/ubuntu/remastersys.gpg.key | apt-key add -<br />gedit /etc/apt/sources.list</code></pre><br />
4. sehingga muncul sourceslist, pada sourceslist masukkan code di bawah ini<br />
<pre><code>deb http://www.remastersys.com/ubuntu precise main</code></pre><br />
5. Save sourceslistnya<br />
6. Masih di root masukkan command:<br />
<pre><code>sudo apt-get update &amp;&amp; sudo apt-get install remastersys remastersys-gui<br /></code></pre><br />
Sehingga akan otomatis proses download. Tunggu sampai proses instalasi selesai.</div>
