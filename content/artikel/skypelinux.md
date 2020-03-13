+++
title = "NgeShare - Cara Menginstal Skype 4.1 di Ubuntu/ Linux Mint"
date = 2012-11-15T04:22:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="630" data-original-width="1200" src="https://3.bp.blogspot.com/-4IHucCagTWU/W-9c0y1PecI/AAAAAAAASb0/iFl-0Q8Do8cgr9uEm9bJigiFA4eOCNdNACLcBGAs/s1600/skype.jpg" /></center><br />
<div style="text-align: justify;">Skype 4.1 baru saja dirilis untuk sistem Linux yang membawa kompatibilitas yang lebih baik untuk Unity dan Gnome Shell. Dalam tutorial ini, saya akan membantu Anda menginstalnya ke dalam Ubuntu/ Linux Mint. Tapi pertama-tama, mari kita lihat beberapa fitur baru dan perubahan dalam rilis terbaru:<br /><br />
<ul style="text-align: justify;"><li>Ngobrol dengan teman menggunakan&nbsp;Windows Live Messenger&nbsp;di Skype</li><li>Masuk menggunakan akun Microsoft tanpa perlu membuat akun Skype baru</li><li>Kualitas video untuk video chatting lebih baik, dll</li></ul><br /><br />
Untuk menginstal Skype 4.1 di Ubuntu 12.10/12.04/Linux Mint 13, buka terminal dan masukkan perintah-perintah untuk platform i386:<br />
<pre><code>sudo apt-get install libxss1<br /><br />cd /tmp<br /><br />wget -c http://goo.gl/XaHpa -O skype-ubuntu-precise_4.1.0.20-1_i386.deb<br /><br />sudo dpkg -i skype-ubuntu*.deb</code></pre><br />
<center><img border="0" src="https://2.bp.blogspot.com/-2qzSvuY4ryQ/UKQK1I-kGrI/AAAAAAAAAGY/XAr1qto178A/s1600/skype-4-1.png" /></center><br />
Versi 64-bit dari Skype 4.1 saat ini tidak tersedia, namun akan ditambahkan ke pos segera setelah tersedia. Berikut adalah trik yang akan membantu Anda menginstal Skype 4.1 dalam versi 64-bit dari Ubuntu / Linux Mint:<br />
- Via terminal menginstal Skype 4.0 (64-bit) melalui terminal dengan perintah ini:<br />
<pre><code>sudo apt-get install skype</code></pre><br />
- Untuk menghapus Skpe 4.1, gunakan perintah ini:<br />
<pre><code>sudo apt-get remove skype</code></pre><br />
- Sekarang memaksa menginstal versi 32-bit dari Skype 4.1 dalam sistem 64-bit dengan perintah:<br />
<pre><code>cd /tmp<br /><br />wget -c http://goo.gl/XaHpa -O skype-ubuntu-precise_4.1.0.20-1_i386.deb<br /><br />sudo dpkg -i --force-architecture skype-ubuntu*.deb</code></pre><br /><br />
<b><a href="https://www.skype.com/en/get-skype/">Download Skype</a></b></div>
