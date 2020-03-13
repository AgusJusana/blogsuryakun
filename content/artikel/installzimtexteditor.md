+++
title = "NgeShare - Install Zim Text Editor 0.58 di Ubuntu dan Linux Mint"
date = 2012-12-18T03:47:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<div style="text-align: justify;">Kini telah dirilis lho Zim versi 0.58, rilis kali ini memuat perbaikan pecegahan terjadinya bug, terutama mencegah terjadinya bug yang menyebabkan tebarkan proses antara aplikasi di Linux. Rilis baru ini memungkinkan pengguna untuk mengekspor persamaan LaTeX dan link interwiki.<br /><br />
Zim adalah (WYSIWYG) grafis editor teks yang ditulis dengan Python dan GTK + yang dikembangkan oleh Jaap Karssenberg yang membawa konsep wiki ke desktop Linux Anda. Zim juga dianggap sebagai jurnal pribadi atau to-do list.<br /><br />
<center><img border="0" src="https://1.bp.blogspot.com/-C4AcDl9c_HM/UM-DYvDmdXI/AAAAAAAAAd8/dCeUfiPKRs8/s1600/zim-equation.png" /></center><br />
Untuk informasi lebih lanjut dan fitur tentang Zim, klik tombol di bawah ini.<br /><br />
<b><a href="http://zim-wiki.org/manual/About.html" target="_blank">More Feature</a></b><br /><br />
Pada artikel ini, kita akan melihat bagaimana cara menginstal Zim dari PPA di Ubuntu/ Linux Mint.<br />
<b><span style="font-size: large;">Instal Zim</span></b><br />
Buka terminal dan masukkan perintah di bawah ini ke dalam terminal:<br />
<pre><code>sudo add-apt-repository ppa:jaap.karssenberg/zim<br /><br />sudo apt-get update<br /><br />sudo apt-get install zim</code></pre><br />
Untuk bug yang dihadapi saat menggunakan software ini, tolong laporkan <b><a href="https://bugs.launchpad.net/~jaap.karssenberg" target="_blank">di sini</a></b>.<br /><br />
<b><span style="font-size: large;">Menghapus Zim</span></b><br />
Untuk menghapus Zim dari sistem anda, jalankan perintah berikut:<br />
<pre><code>sudo apt-get remove zim<br /><br />sudo add-apt-repository --remove ppa:jaap.karssenberg/zim<br /><br />sudo apt-get update<br /></code></pre></div>
