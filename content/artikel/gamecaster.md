+++
title = "NgeShare - Memasang Gamecaster di Linux Ubuntu"
date = 2012-08-12T04:15:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="600" data-original-width="1200" src="https://4.bp.blogspot.com/-gdL1N7WQXEo/XDUkvM9jx9I/AAAAAAAASxs/9fhtS5N2e9kzPJ7ylg-RYQG8s3v64iLhACLcBGAs/s1600/game.png" /></center><br />
<div style="text-align: justify;">Apakah Anda mempunyai niat untuk merekam game yang sedang Anda mainkan di Linux, khususnya Ubuntu? Jika niatan itu ada dalam diri Anda, Anda dapat melakukannya dengan menggunakan sebuah software yang bernama "Gamecaster".<br /><br />
Gamecaster merupakan software yang memiliki fungsi menangkap rekaman real time dari setiap game Linux yang menggunakan ALSA untuk suara dan OpenGL untuk gambar.<br /><br />
Software ini memiliki beberapa fitur yang menarik, berikut ini di antaranya:<ul style="text-align: justify;"><li>Menangkap video HD game Linux yang menggunakan akselerasi OpenGL</li><li>Pilih biner game atau memilih salah satu permainan yang terinstal untuk mulai merekam</li><li>GLC file player.</li><li>Encode file ditangkap GLC. Ke dalam format video WebM</li><li>Pilihan untuk mengubah capture hotkey, bitrate video dan jumlah thread CPU</li><li>Dukungan Ubuntu indikator</li></ul><table cellpadding="0" cellspacing="0" class="tr-caption-container" style="margin-left: auto; margin-right: auto; text-align: center;"><tbody><tr><td style="text-align: center;"><img border="0" src="https://3.bp.blogspot.com/-tNclg5WXbT0/UCbLU-qx_2I/AAAAAAAACMI/WTwBm4Ngbao/s1600/game.jpg" /></td></tr><tr><td class="tr-caption" style="text-align: center;">Tampilan Gamcaster di Ubuntu 12.04</td></tr></tbody></table><br />
Untuk menginstal Gamecaster di Ubuntu 12,04, jalankan perintah di bawah ini:<br />
<pre><code>sudo add-apt-repository ppa:niteshgupta16/gamecaster-stable<br />sudo apt-get update<br />sudo apt-get install gamecaster<br /></code></pre><br />
Untuk menginstal di distro lain, Anda harus mendapatkan rilis tarball terbaru dari Launchpad.<br /><br />Dependensi yang dibutuhkan adalah: ffmpeg, xdotool, GLC, vorbis-tools, mkvtoolnix, python-gmenu, python.<br /><br />Instalasi mungkin membutuhkan dependensi berikut: python-setuptools, python-distutils-ekstra.<br /><br />Untuk menginstal, membongkar tarball, masuk ke folder diekstraksi dan jalankan:<br />
<pre><code>sudo python setup.py install</code></pre><br />Default path instalasi adalah /usr/ local.</div>
