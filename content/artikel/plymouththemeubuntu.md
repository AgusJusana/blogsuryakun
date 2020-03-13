+++
title = "NgeShare - Cara Mengganti Plymouth Theme di Ubuntu"
date = 2012-08-02T14:26:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<div style="text-align: justify;">Pas lagi ngeremaster ubuntu gak lengkap rasanya kalo plymouthnya gak kita ganti. Kalau kita ganti ama plymouth kreasi sendiri rasanya puas and  pastinya bangga, hehehe.... Oke, kali ini ane mau ngasih info tentang cara mengganti Plymouth di Ubuntu. Sebelum ane kasih tau caranya, ane mau ngejelasin apa itu plymouth?<br /><br />
Plymouth adalah tampilan boot splash pada saat memulai Ubuntu seperti pada gambar dibawah ini.<br />
<center><img border="0" data-original-height="377" data-original-width="1600" src="https://1.bp.blogspot.com/-gdAQlPB4CLw/W-uNb-8SSdI/AAAAAAAASOA/LCIQrXlIyUYGtbps2i4Ul06rgbvmn2I9gCLcBGAs/s1600/plymouth.jpg" /></center><br />Tersedia berbagai macam theme plymouth yang bisa diinstall dari repository dan langsung bisa digunakan, berikut ini caranya :<br /><br />
<span style="font-size: large;"><b>Cara Pertama</b></span><br />
1. Buka terminal, CTRL+ALT+T<br />
2. Cari nama paket theme plymouth, dengan menjalankan perintah berikut ini:<br />
<pre><code>apt-cache search plymouth-theme</code></pre><br />
3. Install salah satu theme plymouth dari hasil pencarian contoh install plymouth theme Ubuntu Studio,<br />
<pre><code>sudo apt-get install plymouth-theme-ubuntustudio</code></pre><br />
4. Mengeset default plymouth theme,<br />
<pre><code>sudo update-alternatives --config default.plymouth</code></pre><br />
5. Akan tampil semua plymouth theme yang sudah terinstall, tanda * plymouth theme default.<br />
6. Masukkan nomor plymouth theme untuk mengesetnya sebagai default plymouth.<br />
<center><img border="0" data-original-height="177" data-original-width="924" src="https://1.bp.blogspot.com/-i6Xgl0rS5Kk/W-uJYD0uNqI/AAAAAAAASNs/uK29yKbIL6ILksmKaa1_KjgaPQms-f6WQCLcBGAs/s1600/plymouth.jpg" /></center><br />
<center><img border="0" data-original-height="188" data-original-width="926" src="https://3.bp.blogspot.com/-TrvIqOwhULU/W-uJYM90nGI/AAAAAAAASNo/qUU-DySPfhomxTYBsVHFh7KXyTUbcuCbQCLcBGAs/s1600/playmouth2.jpg" /></center><br />
<center><img border="0" data-original-height="390" data-original-width="1366" src="https://1.bp.blogspot.com/-_ZZuqfASKpw/W-uJhsZSXFI/AAAAAAAASNw/NNSpMbXSvGw4nYMSHxihHAtxeYAxq_vnACLcBGAs/s1600/playmouth3.jpg" /></center><br />
7. Update initramfs<br />
<pre><code>sudo update-initramfs -u</code></pre><br />
8. Tes plymouth theme tanpa restart,<br />
<pre><code>sudo plymouth-preview</code></pre><br />
9. Restart Ubuntu untuk memastikan plymouth tersebut sudah aktif<i>.<br /><br />
<span style="font-size: large;"><b>Cara Kedua</b></span><br />
1. Install Plymouth Manager,<br />
<pre><code>sudo apt-add-repository ppa:mefrio-g/plymouthmanager<br />sudo apt-get update<br />sudo apt-get install plymouth-manager</code></pre><br />
2. Buka Plymouth Manager, Applications-&gt;System Tools-&gt;Plymouth Manager<br /><br />3. Klik tab Themes, pilih salah satu plymouth lalu klik Install<br /><br />4. Restart Ubuntu<br /><br />
Selamat mencoba! 😃</div>
