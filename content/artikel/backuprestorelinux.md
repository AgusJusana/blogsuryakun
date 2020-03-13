+++
title = "NgeShare - Cara Backup/ Restore Paket Dan Aplikasi Ubuntu/ Linux Mint"
date = 2012-11-06T15:54:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="520" data-original-width="900" src="https://4.bp.blogspot.com/-bHvcwdPAxeo/W-7O51fRDrI/AAAAAAAASa0/bHM18jGiAB8IpfifnhI_ULHNvKXxug1KQCLcBGAs/s1600/ubuntucenter.jpg" /></center><br /><div style="text-align: justify;">Dalam tutorial ini, kita akan belajar membuat cadangan (backup) dari semua paket dan aplikasi yang telah diinstal dari repositori atau Ubuntu Software Center di Ubuntu, Linux Mint, atau sistem berbasis Debian.<br /><br />
Tutorial ini akan membantu kamu agar dengan mudah dapat mengembalikan aplikasi setelah menginstal salinan baru dari sistem operasimu tanpa perlu menginstal setiap paket secara terpisah. Dengan hanya beberapa perintah, kamu dapat menyimpan daftar semua aplikasi yang diinstal dan paket dalam sebuah file teks. Kamu dapat melakukan beberapa langkah ini untuk menginstal semua paket secara otomatis.<br />
1. Buka terminal dan buat salinan cadangan dari aplikasi Anda dengan perintah ini:<br />
<pre><code>sudo dpkg --get-selections &gt; backup.txt</code></pre><br />
Sekarang memindahkan file <b>backup.txt</b> ke lokasi lain (USB drive, CD, hard drive eksternal, dll)<br /><br />
2. Setelah instalasi baru Ubuntu/ Linux Mint, <b><i>cd</i></b> ke folder yang berisi file teksmu (<b>backup.txt</b>), kemudian mengembalikan paketmu dengan perintah:<br />
<pre><code>sudo apt-get install aptitude<br />sudo dpkg --clear-selections<br />sudo dpkg --set-selections &lt; backup.txt<br />sudo aptitude install<br /></code></pre><br />
Kemudian ikuti petunjuk yang diberikan.<br /><br />
<b>Note</b>: Kamu juga dapat menggunakan Ubuntu Software Center untuk sinkronisasi dan menginstal ulang aplikasimu pada komputer Ubuntu yang berbeda. Buka Ubuntu Software Center dan kepala ke File Sync&gt; Antara Komputer.</div>
