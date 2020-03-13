+++
title = "NgeShare - Install Microsoft Office 2010 di Ubuntu dan Linux Mint"
date = 2012-12-30T03:46:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="225" data-original-width="225" height="200" src="https://1.bp.blogspot.com/-Qbei9rS22EQ/W--QFRiSMgI/AAAAAAAASc4/oiVwCupF6Gk_zB4tLpYnb7qB_b05VQ5SACLcBGAs/s200/office.jpg" width="200" /></center><br />
<div style="text-align: justify;">Beberapa pemula mungkin merasa sulit untuk menginstal Microsoft Office 2010 di Ubuntu/ Linux Mint menggunakan Wine. Dalam tutorial singkat ini, kita akan mencoba untuk memfasilitasi proses instalasi untuk Anda dengan memberikan semua langkah yang diperlukan, didukung oleh screenshot untuk menjalankan Office 2010 di sistem anda. Tetapi beberapa bug yang mungkin muncul saat menjalankan Office, saya tidak dapat memastikan bahwa semua pengguna dapat mendapatkannya atau tidak.<br /><br />
Tutorial ini berlaku untuk Ubuntu / Linux Mint distribusi berikut:<br /><br />
<ul style="text-align: justify;"><li>Ubuntu 13.04/12.10/12.04/11.10</li><li>Linux Mint 14/13/12</li></ul><br />
<b>1. Install Wine 1.5.x</b><br />
Pertama instal Wine dengan menggunakan perintah berikut:<br />
<blockquote>sudo add-apt-repository ppa:ubuntu-wine/ppa<br />sudo apt-get update<br />sudo apt-get install wine1.5</blockquote><br />
Jalankan perintah ini untuk membuat ".wine" folder tersembunyi di direktori home Anda:<br />
<blockquote class="tr_bq">winecfg</blockquote><br />
Pada jendela yang akan muncul, buka tab <b>"Libraries"</b> dan di bawah pilih <b>"New override for library"</b>, cari dan pilih <b>"riched20"</b> dan klik <b>Add</b>:<br />
<center><img border="0" src="https://1.bp.blogspot.com/-VoGjt9PgmUI/UN9TwRoP6YI/AAAAAAAAApo/Xv1uxbOUaiY/s1600/winecfg.png" /></center><br />
Klik OK untuk menyelesaikan:<br />
<center><img border="0" src="https://3.bp.blogspot.com/-bP7W3dcVcnA/UN9UAt_ODvI/AAAAAAAAApw/iLLulDkKjNE/s1600/winecfg-1.png" /></center><br />
Jika Anda bekerja pada sistem 64-bit dan ingin memasang Wine, jalankan dalam proses 32-bit, Anda dapat menggunakan dua perintah sebelum meluncurkan instalasi Office:<br />
<blockquote class="tr_bq">export WINEPREFIX=$HOME/wine32<br />export WINEARCH=win32</blockquote><br />
<b>2. Install Office 2010</b><br />Buka folder yang berisi file instalasi office 2010, klik kanan file setup.exe dan pilih &nbsp;<b>"Open with Wine ..."</b>:<br />
<center><img border="0" src="https://1.bp.blogspot.com/-N3nW8Tr7spU/UN9UvZ3uL7I/AAAAAAAAAp4/rQO9AbSwQvo/s1600/wine-office2010-7.png" /></center><br />
Instal software ini seperti yang Anda lakukan pada Windows:<br />
<center><img border="0" src="https://2.bp.blogspot.com/-yIGamez_Y4Q/UN9VP8alpWI/AAAAAAAAAqA/Gs0t0HoO_2g/s1600/wine-office2010-1.png" /></center><br />
<center><img border="0" src="https://3.bp.blogspot.com/-vM9f0dE8qrE/UN9VQ0eJgtI/AAAAAAAAAqE/W04SXaIgsrk/s1600/wine-office2010-2.png" /></center><br />
<center><img border="0" src="https://4.bp.blogspot.com/-pfttt9x82lM/UN9VSSQzSII/AAAAAAAAAqQ/pp9ZupjaEYo/s1600/wine-office2010-3.png" /></center><br />
Setelah menginstal Office 2010, buka dasbor Unity untuk mencari Word 2010, PowerPoint 2010, OneNote 2010, Excel 2010, atau Outlook 2010:<br />
<center><img border="0" src="https://3.bp.blogspot.com/-LblNd4yheJc/UN9VgrxFoBI/AAAAAAAAAqY/4v_8nHv7SoA/s1600/wine-office2010-4.png" /></center><br />
Berikut adalah beberapa screenshot:<br />
<center><img border="0" src="https://4.bp.blogspot.com/-HWR-HlWTjyo/UN9WOzWYzyI/AAAAAAAAAqk/DRfOrGMSpLw/s1600/wine-office2010-OneNote.png" /></center><br />
<center><img border="0" src="https://3.bp.blogspot.com/-QhzYuJ072SQ/UN9WQehtUqI/AAAAAAAAAqs/tRAdGljmXVc/s1600/wine-office2010-excel.png.png" /></center><br />
<center><img border="0" src="https://1.bp.blogspot.com/-WluVPglyUnU/UN9WRnKXE6I/AAAAAAAAAq0/1J65zxm7a1o/s1600/wine-office2010-outlook.png" /></center><br />
<center><img border="0" src="https://4.bp.blogspot.com/-i4-IJuWKXNE/UN9WTI29NbI/AAAAAAAAAq8/GowaBW8JCwQ/s1600/wine-office2010-powerpoint.png.png" /></center><br />
<center><img border="0" src="https://4.bp.blogspot.com/-leAgioH--1Y/UN9WUT1ly5I/AAAAAAAAArE/L88FEcSt7CE/s1600/wine-office2010-word.png.png" /></center></div>
