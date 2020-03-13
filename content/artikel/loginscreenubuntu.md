+++
title = "NgeShare - Cara Mengubah Tema Login Screen Ubuntu 12.04"
date = 2012-08-05T15:13:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="604" data-original-width="802" src="https://1.bp.blogspot.com/-XAOQvotCYVI/W-ttgNy9MaI/AAAAAAAASMM/g77lBs8O1V8wfNFKZuVaGWQjFVRxvo37gCLcBGAs/s1600/loginscreenubuntu.jpg" /></center><br />
<div style="text-align: justify;">Pada saat setelah Anda menginstal Linux Ubuntu 12.04, apakah terpikir di benak Anda untuk mengganti tampilan Login Screen pada OS tersebut? Jika Anda memikirkan hal tersebut akan tetapi bingung bagaimana caranya, kami punya solusinya. Berikut solusi atau cara dari kami, mari kita simak bersama.<br /><a name='more'></a><br />Pertama, Anda ketik perintah berikut di Terminal:<br />
<pre><code>sudo cp /usr/share/applications/gnome-appearance-properties.desktop /usr/share/gdm/autostart/LoginWindow<br /></code></pre><br />
Lakukan logout maka kalian akan mendapatkan jendela "Appearance Preferences" pada login screen. Seperti biasa, kalian bisa mengubah wallpaper, tema GTK, ikon, dan lain-lain lewat jendela ini.<br /><br />
Jika sudah selesai, tutup jendela "Appearance Properties" lalu login seperti biasa. Lalu, untuk mencegah agar jendela tersebut tidak muncul lagi ketika login, ketik perintah berikut di Terminal:<br />
<pre><code>sudo unlink /usr/share/gdm/autostart/LoginWindow/gnome-appearance-properties.desktop <br /></code></pre><br />
Tentu saja, semakin banyak tema yang kalian instal maka semakin banyak pula pilihan yang bisa kalian pilih ketika mengubah tampilan login screen. </div>
