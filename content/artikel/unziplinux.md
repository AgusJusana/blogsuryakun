+++
title = "NgeShare - Cara Menggunakan Perintah Unzip di Linux"
date = 2018-12-08T20:24:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="600" data-original-width="1200" src="https://2.bp.blogspot.com/-7skXnir1i88/XDPsrg9ymhI/AAAAAAAASvw/VDZR3SkVNX0KvXJ1ZKvAyhwJciUe3fdSACLcBGAs/s1600/tutorial.jpg" /></center><br />
<div style="text-align: justify;">Setelah sebelumnya saya membagikan tutorial mengenai <a href="https://www.suryadhi.web.id/artikel/ziplinux" target="_blank">cara menggunakan perintah “zip” di Linux</a>, pada kesempatan kali ini, saya akan membagikan tutorial mengenai cara menggunakan perintah “unzip” di Linux. Seperti pada tutorial sebelumnya, tutorial kali ini masih berkaitan dengan kode-kode perintah yang harus dijalankan pada terminal. Oke, tanpa perlu panjang lebar, mari simak tutorialnya berikut ini:<br /><br />
<span style="font-size: large;"><b>Mengekstrak (Unzip) File/ Folder.zip</b></span><br />
Perintah dasar yang dapat digunakan di terminal untuk mengekstrak file/ folder berekstensi “.zip” adalah dengan menggunakan perintah:<br />
<pre><code>unzip filename<br /></code></pre><br />
Cara menggunakannya, misalkan kamu memiliki file/ folder.zip yang bernama heytayo1.zip. Untuk dapat mengekstrak file/ folder.zip tersebut melalui terminal, maka perintah yang harus kamu jalankan adalah dengan:<br />
<pre><code>unzip heytayo1.zip<br /></code></pre><br />
<center><img border="0" data-original-height="466" data-original-width="656" src="https://4.bp.blogspot.com/-QL5rgTPQW1A/XAvDquolQOI/AAAAAAAASo4/gTfk7F9gH4oxzI_YogAzEDp_HKTZm3VqgCLcBGAs/s1600/1.jpg" /></center><br />
<span style="font-size: large;"><b>Mengekstrak (Unzip) Beberapa File/ Folder.zip Sekaligus</b></span><br />Perintah dasar yang dapat digunakan di terminal untuk mengekstrak beberapa file/ folder berekstensi “.zip” sekaligus adalah dengan menggunakan perintah:<br />
<pre><code>unzip ‘*.zip’<br /></code></pre><br />
Cara menggunakannya, misalkan kamu memiliki file/ folder yang bernama heytayo1.zip, heytayo2.zip, dan heytayo3.zip. Untuk dapat mengekstrak beberapa file/ folder tersebut melalui terminal, maka kamu harus menjalankan perintah unzip di atas, dan hasilnya akan seperti tampilan di bawah ini:<br />
<center><img border="0" data-original-height="466" data-original-width="656" src="https://2.bp.blogspot.com/-VrpfOzEeVnY/XAvEMq888cI/AAAAAAAASpA/RnjpZ5muuVIP10hIpIZMuEHvD_uczTK0ACLcBGAs/s1600/2.jpg" /></center><br />
Oh, iya, hati-hati jika menggunakan perintah ini karena akan mengekstrak seluruh file/ folder.zip yang tersimpan pada directory yang sedang kamu buka.<br /><br />
<span style="font-size: large;"><b>Mengetahui Konten/ Isi dari File/ Folder.zip</b></span><br />
Perintah “unzip” tidak hanya berfungsi untuk mengekstrak file/ folder berekstensi “.zip”, melainkan juga dapat digunakan untuk melihat atau mengetahui isi yang ada di dalam file/ folder.zip tersebut. Hal itu dapat dilakukan dengan menggunakan perintah dasar berikut ini:<br />
<pre><code>unzip -l filename.zip</code></pre><br />
Cara menggunakannya, misalnya kamu memiliki file/ folder berekstensi .zip dengan nama heytayo1.zip, maka perintah unzip untuk mengetahui izi dari file .zip tersebut adalah:<br />
<pre><code>unzip -l heytayo1.zip</code></pre><br />
<center><img border="0" data-original-height="466" data-original-width="656" src="https://4.bp.blogspot.com/-vP1YFIbLQhE/XAvEwSjv-xI/AAAAAAAASpI/48Z2vEvr15olQT6IE7dnUT4F1AGKrSVeQCLcBGAs/s1600/3.jpg" /></center><br />
<span style="font-size: large;"><b>Mengetahui Detail Informasi dari File/ Folder.zip</b></span><br />Perintah “unzip” dapat digunakan untuk mengetahui detail informasi yang terdapat pada file/ folder berekstensi “.zip”. Cara mengetahui informasi tersebut adalah dengan menggunakan perintah unzip berikut ini:<br />
<pre><code>unzip -v filename</code></pre><br />
Cara penggunaan dari perintah ini seperti pada tampilan di bawah ini:<br />
<center><img border="0" data-original-height="466" data-original-width="656" src="https://2.bp.blogspot.com/-mtslR_UHBms/XAvFD-xszQI/AAAAAAAASpQ/bM4NRWTUXeYPaaDUiZEP2IiYfdRWJnvxACLcBGAs/s1600/4.jpg" /></center><br />
<span style="font-size: large;"><b>Mengetahui Valid Tidaknya File/ Folder.zip</b></span><br />Perintah “unzip” juga dapat digunakan untuk mengetahui mengenai valid tidaknya file/ folder.zip, artinya perintah ini juga berfungsi untuk menguji pakah file “.zip” tersebut terstruktur dengan benar dan dapat digunakan dengan tepat sebelum mengekstraknya. Adapun perintah “unzip” untuk menjalankan hal tersebut adalah dengan menggunakan perintah berikut:<br />
<pre><code>unzip -t filename</code></pre><br />
Cara penggunaannya seperti contoh di bawah ini:<br />
<center><img border="0" data-original-height="466" data-original-width="656" src="https://4.bp.blogspot.com/-BBw3Rqn76HY/XAvFa2xZAII/AAAAAAAASpY/5Fg0khPmxQUASCF2Cv7LEI--QViblAQyACLcBGAs/s1600/5.jpg" /></center><br />
Oke, sekiranya itu tutorial mengenai cara menggunakan perintah unzip di linux kali ini. Seperti biasa, kalau ada pertanyaan atau saran yang ingin kamu sampaikan kepada saya, kamu bisa menuliskannya di kolom komentar yang terletak di bawah postingan ini. Semoga bermanfaat ya! 😊</div>
