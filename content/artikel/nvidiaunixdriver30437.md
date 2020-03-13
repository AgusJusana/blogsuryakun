+++
title = "NgeShare - Pasang Nvidia Unix Driver 304.37 di Ubuntu dan Mint"
date = 2012-08-21T04:31:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="620" data-original-width="980" src="https://4.bp.blogspot.com/-M9YDAQGuaYU/W-1sWjIy1MI/AAAAAAAASVs/aSbsRr3z6gMnOInzXknpH60zudTO-diKACLcBGAs/s1600/nvidia.jpg" /></center><br />
<div style="text-align: justify;">Nvidia sedang giat-giatnya diperbarui, terbukti dengan hadirnya versi terbaru dari Nvidia yaitu Nvdia versi 304.37. Versi terbaru dari Nvidia ini memiliki beberapa dukungan untuk GPU, berikut ini dukungannya:<br />
<ul style="text-align: justify;"><li>GeForce GTX 680M</li><li>Quadro K1000M</li><li>Quadro K2000M</li><li>Tesla K10</li></ul><br /><br />
Selain itu, Nvidia versi terbaru ini telah melewati beberapa tahap pembaharuan dan perbaikan, Anda dapat melihat apa saja yang telah diperbarui dan diperbaiki di sini.&nbsp;Dalam tutorial ini kita akan menunjukkan cara untuk menginstal driver Nvidia Unix 304,37 di Ubuntu/Linux Mint. Untuk distro Linux lain, yang tidak mendukung instalasi PPA, anda dapat menginstal driver secara manual seperti dijelaskan di bawah:<br /><br />
<b>Instalasi Nvidia driver Unix 304,37</b><br />
Buka terminal di Ubuntu 12.10/12.04/11.10/Linux Mint 13 dan install driver Nvidia dengan perintah ini:<br />
<pre><code>sudo apt-add-repository ppa:xorg-edgers/ppa<br />sudo apt-get update<br />sudo apt-get install nvidia-current nvidia-settings</code></pre><br />
Kemudian reboot sistem anda untuk menyelesaikan instalasi. Untuk instalasi manual, anda dapat ikuti petunjuk ini:<br /><br /><b>systems 32-bit/i386cd /tmp</b><br /><pre><code>wget -O NVIDIA-Linux-x86-304.37.run http://us.download.nvidia.com/XFree86/Linux-x86/304.37/NVIDIA-Linux-x86-304.37.run<br />chmod +x NVIDIA-Linux-x86-304.37.run<br />sudo sh NVIDIA-Linux-x86-304.37.run</code></pre><b>systems 64-bit/amd 64cd /tmp</b><br />
<pre><code>wget -O NVIDIA-Linux-x86_64-304.37.run http://us.download.nvidia.com/XFree86/Linux-x86_64/304.37/NVIDIA-Linux-x86_64-304.37.run<br />chmod +x NVIDIA-Linux-x86_64-304.37.run<br />sudo sh NVIDIA-Linux-x86_64-304.37.run</code></pre></div>
