+++
title = "NgeShare - Pasang atau Upgrade Linux Kernel 3.8.6 di Ubuntu dan Linux Mint"
date = 2013-04-08T10:47:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="900" data-original-width="1600" src="https://2.bp.blogspot.com/-m4fKfOOG87s/W--wTN_gjEI/AAAAAAAASeY/jsJEze9r3xI6gvfDBOcW4dsrNJLknaoxwCLcBGAs/s1600/linuxkernel.jpg" /></center><br />
<div style="text-align: justify;">Pagi ini saya akan membagikan cara memasang atau mengupgrade Linux Kernel 3.8.6 di Ubuntu dan Linux Mint. Bagi yang berminat mencobanya, mari disimak dengan serius artikel ini. Untuk arsitektur i386/amd64, Anda dapat menginstal Linux Kernel 3.8.6 dengan perintah berikut:<br />
<pre><code>cd /tmp<br /><br />wget http://dl.dropbox.com/u/47950494/upubuntu.com/kernel-3.8.6 -O kernel-3.8.6<br /><br />chmod +x kernel-3.8.6<br /><br />sudo sh kernel-3.8.6<br /><br />sudo reboot</code></pre><br />
Untuk sistem berbasis ARM, Anda dapat menginstal kernel 3.8.6 dengan perintah ini:<br />
<pre><code>wget http://dl.dropbox.com/u/47950494/upubuntu.com/arm-kernel-3.8.6 -O arm-kernel-3.8.6<br /><br />chmod +x arm-kernel-3.8.6<br /><br />sudo sh arm-kernel-3.8.6<br /><br />sudo update-grub<br /><br />sudo reboot</code></pre><br />
Untuk informasi mengenai perubaha dan perbaikan Linux Kernel 3.8.6, Anda dapat mengetahuinya <b><a href="http://goo.gl/PgNG5">di sini</a></b>.</div>
