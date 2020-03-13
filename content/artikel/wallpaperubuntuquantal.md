+++
title = "NgeShare - Metode Untuk Mengubah Wallpaper Layar Login di Ubuntu 12.10 (Quantal Quetzal)"
date = 2012-10-17T02:41:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<div style="text-align: justify;">Dalam tutorial ini kita akan melihat dua cara untuk mengubah wallpaper default layar login Anda di Ubuntu 12.10 (Quantal Quetzal). Mengubah gambar latar belakang layar logon akan membuatnya lebih menarik dan memenuhi selera Anda.<br />
<center><img border="0" src="https://1.bp.blogspot.com/-RkuV0SUgTeE/UH22Sc7TFEI/AAAAAAAAEe4/5Qplye-tk3k/s1600/log.jpg" /></center><br />
Pertama-tama, saya ingin memberi tahu Anda bahwa saya telah mencoba untuk mengubah layar logon dengan Ubuntu Tweak Ubuntu 12.10, tapi sayangnya tidak berhasil karena bug. Penulis Ubuntu Tweak telah berjanji bahwa itu akan diperbaiki dalam versi berikutnya dari perangkat lunak. Metode yang diberikan di bawah ini juga bisa diterapkan pada Ubuntu 12.04 Precise Pangolin.<br /><br />
<b><span style="font-size: large;">Metode 1</span></b><br />
Buka terminal dan akses folder / usr / share / latar belakang / dengan perintah ini:<br />
<pre><code>gksu nautilus /usr/share/backgrounds/</code></pre><br />
Tempatkan sekarang wallpaper yang ingin Anda gunakan dalam folder ini:<br />
<center><img border="0" src="https://2.bp.blogspot.com/-kcQ2v392lCo/UH22rT4E_nI/AAAAAAAAEfA/TjAJAqHBicU/s1600/log2.png" /></center><br />
Kemudian klik kanan pada ruang kosong pada desktop Anda dan pilih <b>"Change Desktop Background"</b>. Pada jendela Penampilan, pilih <b>"Folder Picture"</b> dari menu dropdown dan pilih wallpaper yang telah Anda ditempatkan di&nbsp;folder&nbsp;/usr/share/backgrounds / :<br />
<center><img border="0" src="https://2.bp.blogspot.com/-DWeKxiK-Dzk/UH221gvvuZI/AAAAAAAAEfI/Mku1YqXU_MU/s1600/log3.png" /></center><br />
Log out sekarang untuk menguji layar login. Satu-satunya kelemahan dengan metode ini adalah bahwa Anda tidak dapat mengatur wallpaper yang berbeda untuk kedua desktop dan layar logon.<br /><br />
<b><span style="font-size: large;">Metode 2 (Rekomendasi)</span></b><br />
Buka terminal dan jalankan perintah ini untuk mendapatkan akses root:<br />
<pre><code>sudo -i</code></pre><br />
Biarkan sekarang lightdm untuk membuat sambungan dengan Xserver dengan perintah ini:<br />
<pre><code>xhost +SI:localuser:lightdm</code></pre><br />
Anda sekarang harus masuk sebagai lightdm:<br />
<pre><code>su lightdm -s /bin/bash</code></pre><br />
Nonaktifkan sekarang "draw-user-backgrounds" dan "draw-grid" dengan perintah:<br />
<pre><code>gsettings set com.canonical.unity-greeter draw-user-backgrounds 'false'<br />gsettings set com.canonical.unity-greeter draw-grid 'false'</code></pre><br />
Sekarang Anda dapat mengatur wallpaper kustom Anda dengan perintah ini:<br />
<pre><code>gsettings set com.canonical.unity-greeter background '/path/to/wallpaper.png'</code></pre><br />
Ganti "/path/to/wallpaper.png" dengan path lengkap ke wallpaper Anda. Anda sekarang dapat logout dan menguji wallpaper login Anda.<br /><br />
Jika Anda memilih untuk mengembalikan pengaturan default, jalankan urutan perintah:<br />
<pre><code>sudo -i<br /><br />xhost +SI:localuser:lightdm<br /><br />su lightdm -s /bin/bash<br /><br />gsettings reset com.canonical.unity-greeter draw-user-backgrounds<br /><br />gsettings reset com.canonical.unity-greeter draw-grid<br /><br />gsettings reset com.canonical.unity-greeter background<br /><br />exit<br /><br />exit</code></pre></div>
