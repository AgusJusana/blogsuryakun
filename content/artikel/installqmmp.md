+++
title = "NgeShare - Install QMMP di Linux"
date = 2018-11-19T08:47:00Z
tags = ["tutorial"]
comments = true
+++

<center><img border="0" data-original-height="600" data-original-width="1200" src="https://1.bp.blogspot.com/-csfYod6AOZM/XDWRwm8pokI/AAAAAAAAS2Y/2xh1ijog_YsipG12724KklIjgqd8tq_3QCLcBGAs/s1600/tutorial.jpg" /></center><br />
<div style="text-align: justify;">Yosh, kali ini saya akan membagikan tutorial mengenai cara memasang atau menginstall "QMMP" di Linux. Tapi, wait, sebenarnya "QMMP" itu apa sih? Oke, saya jelaskan terlebih dahulu secara singkat ya (hehehe...). QMMP adalah sebuah aplikasi pemutar musik (audio) yang memiliki user interface seperti winamp atau xmms (selengkapnya ada <a href="http://qmmp.ylsoftware.com/" target="_blank"><b>di sini</b></a>). Jadi, kalau kamu memasang aplikasi ini di Linuxmu, kamu mungkin akan kembali mengingat <strike>mantan</strike> <a href="https://www.winamp.com/" target="_blank"><b>winamp</b></a> yang dulu pernah menjadi pemutar musik paling populer di Windows.<br /><br />
Oke, tanpa perlu panjang lebar lagi, mari simak tutorial berikut ini:<br />
1. Buka terminal.<br />
2. Kemudian, masukkan beberapa perintah di bawah ini ke dalam terminal:<br />
<pre><code>sudo add-apt-repository ppa:forkotov02/ppa<br /><br />sudo apt-get update<br /><br />sudo apt-get install qmmp qmmp-plugin-pack</code></pre><br />
3. Tunggu hingga proses instalasi selesai. 😊<br />
<table cellpadding="0" cellspacing="0" class="tr-caption-container" style="margin-left: auto; margin-right: auto; text-align: left;"><tbody><tr><td style="text-align: center;"><img border="0" data-original-height="476" data-original-width="800" src="https://2.bp.blogspot.com/-uZKBAGSZZMo/W_IVQdDWbXI/AAAAAAAASgY/3r1DAokk5ok6l3ttK1a4RxFHevesHJOGQCLcBGAs/s1600/qmmp.jpg" /></td></tr><tr><td class="tr-caption" style="text-align: center;">Tampilan QMMP</td></tr></tbody></table><br />
<b>Uninstall QMMP</b><br />
Jika kamu ingin menguninstall aplikasi ini, cukup masukan perintah di bawah ini ke dalam terminal:<br />
<pre><code>sudo apt-get remove --autoremove qmmp qmmp-plugin-pack</code></pre><br />
Oke, itu sekiranya tutorial kali ini. Bila ada pertanyaan atau saran yang ingin kamu sampaikan, tuliskan saja di kolom komentar ya! Semoga bermanfaat... 😁</div>
