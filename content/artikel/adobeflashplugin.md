+++
title = "NgeShare - Cara Menginstall Adobe Flash Plugin di Ubuntu 13.04"
date = 2013-07-08T05:55:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<div dir="ltr" style="text-align: left;" trbidi="on"><div class="separator" style="clear: both; text-align: justify;"><br /></div><div style="text-align: justify;">Suatu ketika saat saya sedang menginstal Adobe Flash di Ubuntu 13.04 melalui Ubuntu Software, saya menemui kendala yang cukup menyulitkan. Kendala tersebut terlihat pada gambar di bawah ini.</div><a name='more'></a><div style="text-align: justify;"><br /></div><div style="text-align: center;"><a href="http://3.bp.blogspot.com/-63QaaCxSoPI/UdnvOpYKRbI/AAAAAAAACkY/N5NTR_tYHV4/s1600/install_redup.png" style="margin-left: 1em; margin-right: 1em;"><img border="0" src="https://3.bp.blogspot.com/-63QaaCxSoPI/UdnvOpYKRbI/AAAAAAAACkY/N5NTR_tYHV4/s1600/install_redup.png" /></a></div><div style="text-align: justify;"><br /></div><div style="text-align: justify;">Terlihat bahwa tombol install tersebut nampak redup atau tidak seperti biasanya, yaitu tulisan install biasanya bewarna hitam. Itu berarti Adobe Flash tidak dapat diinstal di Ubuntu saya. Bingung bagaimana cara mengatasinya, alih-alih saya mencoba mencari solusinya dengan blusukan di mbah google. Dan wala...akhirnya ketemu juga. </div><div style="text-align: justify;"><br /></div><div style="text-align: justify;">Saya menemukan perintah untuk mengatasi masalah ini. Ini dia perintah yang dapat memecahkan permasalahan tersebut. Cukup memasukkannya ke dalam terminal dan tunggu hingga proses selesai.</div><div style="text-align: justify;"><br /></div><div style="text-align: justify;">Perintah 1:</div><div style="text-align: left;"><blockquote class="tr_bq">sudo add-apt-repository "deb http://archive.canonical.com/ $(lsb_release -sc) partner</blockquote></div><div style="text-align: justify;">Perintah 2:</div><div style="text-align: justify;"><blockquote class="tr_bq">sudo apt-get update &amp;&amp; sudo apt-get install flashplugin-installer</blockquote></div><div style="text-align: justify;">Setelah proses selesai, cek kinerja adobe flash tersebut di http://www.adobe.com/software/flash/about/ untuk mengetes apakah berhasil terinstall atau tidak.</div><div style="text-align: justify;"><br /></div><div style="text-align: justify;">Jika Anda memiliki masalah yang sama seperti saya ini, Anda dapat mencobanya. Lebih mudah ketika Anda telah mengganti repo Anda menjadi kambing.ui.ac.id karena Anda tinggal memasukkan perintah:</div><div style="text-align: justify;"><blockquote class="tr_bq">sudo apt-get install flashplugin-installer</blockquote></div><div style="text-align: justify;">Itulah sekiranya yang dapat saya tuliskan pada posting ini. Bila ada kesalahan terhadap penulisan, saya mohon maaf. Semoga bermanfaat... 😁</div><div style="text-align: justify;"></div></div>