+++
title = "NgeShare - Resize Banyak Gambar Sekaligus di Linux "
date = 2016-06-09T18:42:00Z
tags = ["tutorial"]
comments = true
+++

<center><img border="0" data-original-height="600" data-original-width="1200" src="https://3.bp.blogspot.com/-ynZmPrzxy0I/XFzcJzNmKUI/AAAAAAAATGw/o8rImR5ElrwtZlR95wSVu2E5n7gdRt3cwCLcBGAs/s1600/resize.png" /></center><br />
<div style="text-align: justify;">Ada kalanya kita perlu mengubah ukuran (piksel) gambar untuk keperluan <i>blogging</i> misalnya, atau untuk <i>editing</i> sebelum di<i>share</i> ke sosmed. Di Linux, sudah ada <i>tool</i> yang mumpuni untuk me-<i>resize</i> gambar, salah satunya adalah <a href="http://gimp.org/" target="_blank">Gimp</a>. Nah bagaimana kalau gambar yang mau di-<i>resize</i> ada banyak? Kalau harus di-<i>resize</i> satu per satu tentunya akan merepotkan.<br /><br />
Tenang saja, di Linux sudah ada program bernama <b>ImageMagick</b> yang bisa dipakai untuk keperluan tersebut. Linux yang saya gunakan di sini adalah Ubuntu, install ImageMagick lewat terminal dengan perintah<br />
<pre><code>sudo apt-get install imagemagick</code></pre><br />
Teman-teman juga dapat menggunakan distro Linux selain Ubuntu, asalkan distro tersebut dapat diinstall ImageMagick.<br /><br />
Saya mempunyai beberapa gambar yang saya simpan di <b>/home/linuxluv/Pictures/ori</b><br />
<center><img border="0" height="234" src="https://c8.staticflickr.com/8/7342/27487083951_bf773d19f4_o.jpg" width="640" /></center><br />
Dapat dilihat pada screenshot di atas saya mempunyai beberapa gambar yang salah satu di antaranya berukuran 2.448 x 3.264 piksel. Untuk me-resize semua gambar yang ada di /home/linuxluv/Pictures/ori<br />
1. Buka terminal, masuk ke /home/linuxluv/Pictures/ori<br />
<pre><code>cd /home/linuxlu/Pictures/ori</code></pre><br />
<center><img border="0" src="https://c2.staticflickr.com/8/7012/27559379805_570dc9f959_o.png" /></center><br />
2. Untuk me-resize semua gambar sekaligus eksekusi perintah berikut lewat terminal:<br />
<pre><code>mogrify -resize 75% *</code></pre><br />
perintah di atas akan mengubah ukuran semua gambar menjadi 75% lebih kecil dari ukuran gambar aslinya<br /><br />
atau bila ingin mengubah ukuran gambar ke ukuran tertentu, misalnya 640 x 480 piksel, eksekusi perintah:<br />
<pre>mogrify -resize '640x480' *</code></pre><br />
perintah di atas akan mengubah ukuran semua gambar menjadi 480 x 640 piksel<br /><br />
bisa juga mengubah ukuran gambar berdasarkan lebarnya, misalnya menggunakan perintah berikut<br />
<pre><code>mogrify -resize width='400' *</code></pre><br />
perintah di atas akan me<i>resize </i>gambar agar lebarnya menjadi 400 piksel, sedangkan tinggi gambar akan menyesuaikan secara otomatis sesuai rasio panjang x lebarnya<br /><br />bisa juga mengubah ukuran gambar berdasarkan tingginya, misalnya menggunakan perintah berikut <br /><pre style="text-align: justify;">mogrify -resize height='600' *</pre>perintah di atas akan me<i>resize </i>gambar agar tingginya menjadi 600  piksel, sedangkan lebar gambar akan menyesuaikan secara otomatis sesuai  rasio panjang x lebarnya<br /><br />
Perintah di atas juga dapat digunakan untuk me-resize satu file gambar dengan menuliskan nama file nya, misal<br />
<pre><code>mogrify -resize 75% gambar1.png</code></pre><br />
<a href="http://www.daredevel.com/resize-multiple-images-using-linux/" target="_blank">sumber</a></div>
