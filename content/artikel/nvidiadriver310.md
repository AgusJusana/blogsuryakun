+++
title = "NgeShare - Cara Install Nvidia Driver 310.14 di Ubuntu dan Linux Mint"
date = 2013-02-08T13:48:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="349" data-original-width="620" src="https://4.bp.blogspot.com/-dqhCnBuFCIE/W--Tfej3EaI/AAAAAAAASdk/-zxW7VTE6IYZhQqoh4HoqEWToKpXEjmiACLcBGAs/s1600/Nvidia.jpg" /></center><br />
<div style="text-align: justify;">Setelah disibukkan dengan template blog ini, kali ini saya akan ngeshare lagi hal-hal yang sepertinya akan berguna untuk saya dan Anda. Kali ini saya akan ngeshare tutorial untuk menginstal driver Nvidia 310.14 beta pada linux Ubuntu 12.10/12.04 dan linux Mint 13. Tidak perlu basa-basi, mari kita simak tutorial berikut ini:<br /><br />
Buka terminal dan jalankan perintah di bawah ini:<br />
<blockquote class="tr_bq">sudo add-apt-repository ppa:xorg-edgers/ppa<br />sudo apt-get update<br />sudo apt-get install nvidia-current nvidia-settings</blockquote><br />
Untuk instalasi manual, lakukan hal berikut:<br /><br />
Buka terminal dan jalankan perintah ini:<br />
<blockquote class="tr_bq">cd &amp;&amp; wget http://dl.dropbox.com/u/47950494/upubuntu.com/nvidia-310-14<br />chmod +x nvidia-310-14</blockquote><br />
Tekan CTRL + ALT + F3 dan gunakan kredensial login Anda.<br />
Hentikan xserver dengan perintah ini:<br />
<blockquote class="tr_bq">sudo service lightdm stop</blockquote><br />
Instal driver dengan perintah ini:<br />
<blockquote class="tr_bq">cd &amp;&amp; sudo sh nvidia-310-14</blockquote><br />
Terakhir, reboot sistem Anda:<br />
<blockquote class="tr_bq">sudo reboot</blockquote></div>
