+++
title = "NgeShare - Cara Mengenkripsi USB Drive di Lubuntu 18.04"
date = 2018-09-22T12:35:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="600" data-original-width="1200" src="https://4.bp.blogspot.com/-Bb57cgTHNTs/XDWV9BAIPmI/AAAAAAAAS28/uLzw6ZYNKpwuiaplLOo5S3N1nH1OjD-ZQCLcBGAs/s1600/tutorial.jpg" /></center><br />
<div style="text-align: justify;">Apakah kalian pernah mendengar istilah 'enkripsi'? Mungkin beberapa dari kalian telah mengetahui arti dari istilah tersebut. 'Mengamankan', yaps, enkripsi dapat dikatakan sebagai istilah kata yang memiliki arti, yaitu mengamankan data menggunakan kode-kode atau sandi tertentu. Istilah ini sangat populer digunakan di dunia teknologi, apalagi sejak maraknya sosial media, karena sebagian besar sosial media menggunakan sistem enkripsi pada fitur chatting mereka. Hal itu dilakukan agar data pengguna dapat terlindungi dan hanya dapat diakses oleh pengguna tersebut saja. Namun, tidak hanya pada sosial media, enkripsi juga diaplikasikan pada beberapa aplikasi di PC dengan tujuan agar dapat melindungi data privasi penggunanya.<br /><br />
Bicara masalah enkripsi, di sini saya akan membagikan tips mengenai cara mengenkripsi USB Drive di Lubuntu 18.04. Melalui tips ini, kamu yang saat ini mungkin sedang menggunakan OS Lubuntu 18.04 atau OS Linux lainnya dapat mengamankan data pada USB Drive milikmu dari kejahilan orang lain (hehehe...). Itu artinya, melalui tips ini nanti, hanya kamu seorang yang dapat mengakses data pada USB Drive yang telah dienkripsi tersebut. Oke, tanpa perlu panjang lebar, langsung saja simak tips berikut ini.<br /><br />
1. Buka terminal (CTRL+ALT+T), kemudian jalankan perintah di bawah ini dan tunggu hingga proses install selesai.<br />
<pre><code>sudo apt-get install gnome-disk-utility cryptsetup -y</code></pre><br />
2. Ketika proses install selesai, cari aplikasi 'Disks' pada menu.<br />
<center><img border="0" data-original-height="559" data-original-width="800" src="https://1.bp.blogspot.com/-Hn2mAp0zv4U/W6XOAxuRMVI/AAAAAAAARrE/VN-Rke3aNYM2seBljUmT7vS0_3fkUP30gCLcBGAs/s1600/Screenshot%2Bfrom%2B2018-09-21%2B13-05-23.png" /></center><br />
3. Jalankan aplikasi tersebut, dan akan muncul tampilan seperti di bawah ini. Kemudian pilih device USB Drive-mu.<br />
<center><img border="0" data-original-height="728" data-original-width="802" src="https://4.bp.blogspot.com/-lUGRManv79Y/W6XOW2k4NoI/AAAAAAAARrM/4TSs0X283e4h27P8AtycA6MRtbGPE2sbQCLcBGAs/s1600/Screenshot%2Bfrom%2B2018-09-21%2B13-06-24.png" /></center><br />
4. Setelah itu, pilih fitur 'Unmount selected partition'.<br />
<center><img border="0" data-original-height="728" data-original-width="802" src="https://3.bp.blogspot.com/-Yd-bNzuCJyc/W6XOvNZJveI/AAAAAAAARrU/6MUtR3KfeL88zVYtkizugWaUNLRJm9xlACLcBGAs/s1600/Screenshot%2Bfrom%2B2018-09-21%2B13-07-29.png" /></center><br />
5. Pada fitur 'Unmount selected partition', pilih fitur 'Format Partition...'. <span style="color: #0b5394;">Sebelum melakukan langkah ini, pastikan kamu telah mem-back-up semua data dari USB Drive-mu, karena langkah ini akan menghapus semua data dari USB Drive tersebut.<br />
<center><img border="0" data-original-height="728" data-original-width="802" src="https://4.bp.blogspot.com/-zrccjJMmBb0/W6XPJnwA-_I/AAAAAAAARrc/qPbFPszsFu8waWm9xtOxmP9AjepEqimDQCLcBGAs/s1600/Screenshot%2Bfrom%2B2018-09-21%2B13-08-19.png" /></center><br />
6. Dari menu 'Format Partition...', akan muncul tampilan seperti berikut ini.<br />
<center><img border="0" data-original-height="423" data-original-width="600" src="https://2.bp.blogspot.com/-aOcJR5WucuY/W6XPWNtpQ7I/AAAAAAAARrg/wWOaMe_o9aghRMJthgt_AB525CuEUpIHgCLcBGAs/s1600/Screenshot%2Bfrom%2B2018-09-21%2B13-09-36.png" /></center><br />
7. Pada tampilan ini, kamu ketik nama USB Drive-mu pada 'Volume Name', lalu pilih 'Internal disk for use with...' dan pilih 'Password protect volume (LUKS)', kemudian klik 'Next'.<br />
<center><img border="0" data-original-height="423" data-original-width="600" src="https://2.bp.blogspot.com/-W9ixkyl7Jo4/W6XQFGMdWwI/AAAAAAAARrs/eEATml1UbXUitaXAoKGNyCLE72DlpTQKwCLcBGAs/s1600/Screenshot%2Bfrom%2B2018-09-21%2B13-14-19.png" /></center><br />
8. Muncul tampilan berikutnya yang mengharuskan kamu untuk menuliskan password sesuai dengan keinginanmu. Setelah itu klik 'Next' dan tunggu hingga proses selesai.<br />
<center><img border="0" data-original-height="423" data-original-width="600" src="https://2.bp.blogspot.com/-hhX6pHi4-1U/W6XQaZOEg-I/AAAAAAAARr0/Pwfl5m5_SfYBxWmGAXx_2WzMxsZaZbtiwCLcBGAs/s1600/Screenshot%2Bfrom%2B2018-09-21%2B13-15-15.png" /></center><br />
9. Ketika muncul tampilan seperti di bawah ini, maka proses format partition dan enkripsi telah selesai.<br />
<center><img border="0" data-original-height="728" data-original-width="802" src="https://1.bp.blogspot.com/-B9xWYEv8jn0/W6XQsb3iANI/AAAAAAAARsA/vkDmYzBDJkEO5c_Jk3dkze3N4-Nmn4oMACLcBGAs/s1600/Screenshot%2Bfrom%2B2018-09-21%2B13-16-40.png" /></center><br />
10. Setelah itu, pilih 'Eject this disk' dan cabut USB Drive dari PC-mu.<br />
<center><img border="0" data-original-height="725" data-original-width="799" src="https://3.bp.blogspot.com/-d6QQZh66Ld0/W6XRLJaisaI/AAAAAAAARsI/bDrKgXURNHIBBGTnNyUKXvSjR-MFg3PwgCLcBGAs/s1600/Screenshot%2Bfrom%2B2018-09-21%2B13-17-00.png" /></center><br />
11. Pasang kembali USB Drive tersebut ke PC, nantinya akan muncul tampilan seperti berikut ini. Pada tampilan ini, kamu ketikan password kamu tadi, kemudian klik 'Connect'.<br />
<center><img border="0" data-original-height="302" data-original-width="477" src="https://3.bp.blogspot.com/-xdNR_TLb-yk/W6XRmgMc4rI/AAAAAAAARsQ/gt3XEveI38cWiqcZJ-3AD2t32x2Z8UywACLcBGAs/s1600/Screenshot%2Bfrom%2B2018-09-21%2B13-18-07.png" /></center><br />
12. Jika password yang kamu ketikan benar, akan muncul tampilan seperti di bawah ini.<br />
<center><img border="0" data-original-height="409" data-original-width="402" src="https://1.bp.blogspot.com/-i2clcoS273E/W6XR7MKs_TI/AAAAAAAARsY/IYN9FkiwhBsBsN4OX9gyad4YDODBcAHvgCLcBGAs/s1600/Screenshot%2Bfrom%2B2018-09-21%2B13-19-15.png" /></center><br />
13. Setelah selesai proses di atas, barulah kamu dapat mengakses data pada USB Drive milikmu. 😁<br />
<center><img border="0" data-original-height="728" data-original-width="1366" src="https://4.bp.blogspot.com/-YdkqiWLbj4s/W6XSVgvOz1I/AAAAAAAARsg/rVFgeLzT6LIDBdPgxK1B8Ze1q8VrX6MjACLcBGAs/s1600/Screenshot%2Bfrom%2B2018-09-21%2B13-20-03.png" /></center></div>
