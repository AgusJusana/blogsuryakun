+++
title = "NgeShare - Install MAME (Multiple Arcade Machine Emulator) di Ubuntu 12.10/12.04 dan Linux Mint 13"
date = 2012-10-05T05:03:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<div style="text-align: justify;">MAME (Multiple Arcade Machine Emulator) adalah sebuah software emulasi yang memungkinkan pengguna untuk bermain game arcade klasik dalam komputer modern dan platform. Emulator ini mendukung lebih dari 7000 game arcade + video dari era 1970-an sampai sekarang.<br />
<center><img border="0" src="https://4.bp.blogspot.com/-5g8rvUxUY4E/UG4G_EWEIUI/AAAAAAAAEAU/HWn2gt39dSg/s1600/mame2.png" /></center><br />
Dalam tutorial ini kami akan membantu anda menginstal MAME dalam distribusi Linux berikut:<br /><br />
<ul style="text-align: justify;"><li>Ubuntu 12.10 (Quantal Quetzal)</li><li>Ubuntu 12.04 (Precise Pangolin)</li><li>Linux Mint 13</li></ul><br />
<b>1.&nbsp;Instalasi&nbsp;MAME</b><br />
Buka terminal bawah Ubuntu / Linux Mint dan menjalankan perintah ini untuk menginstal MAME:<br />
<pre><code>sudo apt-get install mame mame-tools gnome-video-arcade sdlmame sdlmame-tools</code></pre><br />
<b>2.&nbsp;Konfigurasi&nbsp;MAME</b><br />
Mulai MAME&nbsp;sekarang&nbsp;dengan perintah ini sehingga folder tersembunyi (<b>.mame</b>) Dibuat dalam direktori home Anda yang akan berisi semua pengaturan emulator:<br />
<pre><code>mame<br /></code></pre><br />
Sekarang Anda dapat menutup emulator. Jalankan perintah ini untuk membuat file konfigurasi untuk MAME:<br />
<pre><code>cd ~/.mame &amp;&amp; mame -cc</code></pre><br />
<b>mame.ini</b>" file akan dibuat dalam folder&nbsp;<b>~/.mame</b>. Edit sekarang file ini dengan perintah ini:<br />
<pre><code>gedit ~/.mame/mame.ini<br /></code></pre><br />
Untuk Linux Mint:<br />
<pre><code>pluma ~/.mame/mame.ini</code></pre><br />
Dalam "<b>rompath</b>", Anda dapat mengatur ROM Anda sendiri jalur direktori atau meninggalkan jalur baku:<br />
<center><img border="0" src="https://1.bp.blogspot.com/--jzE7MNSeWc/UG4HVA-jzDI/AAAAAAAAEAc/zksaOGd6aoM/s1600/mame3.png" /></center><br />
Selanjutnya, buat direktori dalam folder&nbsp;<b>~/.mame</b>:<br />
<ul style="text-align: justify;"><li>nvram</li><li>sta</li><li>roms</li><li>memcard</li><li>inp</li><li>comments</li><li>snap</li><li>diff</li></ul><br />
Anda dapat membuat mereka semua dengan perintah ini:<br />
<pre><code>mkdir ~/.mame/nvram memcard roms inp comments sta snap diff<br /></code></pre><br />
Anda dapat mengakses folder rom dengan perintah ini untuk menempatkan roms Anda download di:<br />
<pre><code>nautilus ~/.mame/roms<br /></code></pre><br />
Adapun kontrol pemutar, Anda dapat dengan mudah mengkonfigurasi mereka dari antarmuka utama MAME (<b>Configure General Inputs</b>):<br />
<center><img border="0" src="https://3.bp.blogspot.com/-CH_adsamRCo/UG4HkeMCGXI/AAAAAAAAEAk/LLydkYDw4_c/s1600/mame4.png" /></center><br />
<b>Note:</b> Sementara permainan dengan MAME, Anda dapat keluar dari mode fullscreen dengan menekan ALT + Enter.&nbsp;</div>
