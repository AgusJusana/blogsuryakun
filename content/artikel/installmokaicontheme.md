+++
title = "NgeShare - Install Moka Icon Theme di Ubuntu"
date = 2013-09-01T11:10:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" src="https://4.bp.blogspot.com/-zqtlsnptf78/UiK90ox-mCI/AAAAAAAADBc/0xaDQdxTEio/s1600/moka_icon_theme_preview.png" /></center><br />
<div style="text-align: justify;">Ye....balik lagi di suryapersonal. Kali ini ane mau bagi-bagi tentang menginstal Icon Theme yang keren buat Linux agan khusunya Ubuntu. Icon theme yang mau ane bagi ini bernama Moka. Pasti beberapa dari agan sudah mendengar tentang icon theme ini. Moka adalah sebuah icon theme yang dirancang secara sederhana, jelas dan konsisten sebagai pemanis di dekstop <span class="" id="result_box" lang="id"><span class="hps">Unity</span><span class="">,</span> <span class="hps">Gnome</span><span class="">,</span> <span class="hps">Cinnamon</span> <span class="hps">dan</span> <span class="hps">lainnya (untuk KDE belum tersedia)</span></span>.<br /><br />
Icon theme ini didistribusikan di bawah GNU GPL versi 3. Sayangnya ketika agan telah menginstall icon theme ini, akan terjadi beberapa icon yang tidak muncul, namun jangan khawatir, tidak begitu banyak icon yang tidak akan muncul. Dan tetap keren ketika agan menggunakannya.<br />
<center><img border="0" src="https://4.bp.blogspot.com/-7feQZTpBF8Y/UiK8bF_UaOI/AAAAAAAADBI/eAzRgSAJkC0/s1600/moka_blue.png" /></center><br />
<center><img border="0" src="https://3.bp.blogspot.com/-iMJ0vdXQ2hY/UiK824PdmcI/AAAAAAAADBQ/qdBXzbC1Ooo/s1600/moka_dark.png" /></center><br />
Jika agan tertarik untuk menginstall dan menggunakannya, cukup masukkan beberapa perintah di bawah ini ke dalam terminal (Ctrl+Alt+T):<br />
<pre><code>sudo add-apt-repository ppa:snwh/moka-icon-theme-daily<br /><br />sudo apt-get update<br /><br />sudo apt-get install moka-icon-theme<br /><br />sudo apt-get install moka-icon-theme-blue<br /><br />sudo apt-get install moka-icon-theme-dark</code></pre><br />
Bagi agan yang tidak menggunakan Ubuntu melainkan linux lain tak perlu khawatir, agan tetap dapat menginstallnya dengan menggunakan perintah di bawah ini:<br />
<pre><code>wget -O moka-icon.deb http://goo.gl/6eCp4H<br /><br />wget -O moka-icon-blue.deb http://goo.gl/81Gztk<br /><br />wget -O moka-icon-dark.deb http://goo.gl/JTEUFe<br /><br />sudo dpkg -i moka-icon.deb moka-icon-blue.deb moka-icon-dark.deb<br /><br />rm moka-icon.deb moka-icon-blue.deb moka-icon-dark.deb</code></pre></div>
