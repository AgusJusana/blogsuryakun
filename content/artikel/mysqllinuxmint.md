+++
title = "NgeShare - Menginstall MySQL di Linux Mint 15"
date = 2013-07-28T04:57:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="600" data-original-width="1200" src="https://4.bp.blogspot.com/-qVLfxNyjaMs/XF5J34YiG8I/AAAAAAAATIg/ptH2TIPNimE0ILfovNhpOQ_ly3ahRqC6ACLcBGAs/s1600/mysql.png" /></center><br />
<div style="text-align: justify;">Kali ini ane akan berbagi tentang bagaimana cara menginstall MySQL di Linux Mint 15. Semoga apa yang ane lakuin ini dapat sekiranya membantu Agan dalam memanajemen database server di linux, khususnya di Linux Mint. Yang pertama Agan lakukan dalam proses instalasi ini adalah Agan buka Synaptic Package Manager.<br />
<center><img border="0" src="https://1.bp.blogspot.com/-SC8vdLvv5Fk/UfQ8LvfmBxI/AAAAAAAACus/TdWuS6xu2fw/s1600/sql.png" /></center><br />
Setelah itu, cari <i>'mysql-server'</i> untuk lebih mudahnya ketikkan <i>'mysql-server'</i> (tanpa tanda kutip) di kotak quick search.<br />
<center><img border="0" src="https://3.bp.blogspot.com/-T5H_uBf7ssA/UfQ8hxqZuGI/AAAAAAAACu0/rccnfO39o_c/s1600/1sql.png" /></center><br />
Kalau udah ketemu, klik kanan pada <i>'mysql-server'</i>. Kemudian muncul menu pop up, pada menu pop up, klik kanan, pilih Mark For Installation.
<center><img border="0" src="https://4.bp.blogspot.com/-Bf9IQTVnrAo/UfQ8_g3YPMI/AAAAAAAACu8/QlVhSM9uuQU/s1600/2sql.png" /></center><br />
Dan Agan klik Apply untuk menginstalnya.<br />
<center><img border="0" src="https://3.bp.blogspot.com/-X0J9pcLZJEo/UfQ9v3GXJ3I/AAAAAAAACvE/olxxmpUsPGU/s1600/3sql.png" /></center><br />
Tunggulah hingga proses instalasi selesai.<br />
<center><img border="0" src="https://1.bp.blogspot.com/-MrFvqieEKdg/UfQ-02zmwTI/AAAAAAAACvU/kRtT7rgE3Y0/s1600/4sql.png" /></center><br />
Jika proses instalasi <i>'mysql-server'</i> telah selesai, sekarang Agan cari <i>'mysql-client'</i>, lakukan proses instalasi yang sama terhadap <i>'mysql-client'</i>.<br />
<center><img border="0" src="https://2.bp.blogspot.com/-TT1HIGKj-IA/UfQ_Xa9mFGI/AAAAAAAACvc/R5sE4MJnNHc/s1600/8sql.png" /></center><br />
Saat proses penginstalan, Agan akan diminta untuk memasukkan sebuah password sebagai <i>'root'</i>-nya. Masukkan sesuai keinginan Agan, terus klik Forward.<br />
<center><img border="0" src="https://2.bp.blogspot.com/-M6UK4lj1ELg/UfRAHUAtXyI/AAAAAAAACvo/PiE_quDjvjQ/s1600/5sql.png" /></center><br />
Setelah semua proses selesai, Agan masuk ke terminal <strike>bus</strike>, ketik <i>'mysql -u root -p'</i> (tanpa tanda kutip). Dan wala...MySQL telah siap sedia untuk digunakan, hehehe....<br />
<center><img border="0" src="https://3.bp.blogspot.com/-zQot3dK8r1k/UfRBGg0znfI/AAAAAAAACv0/zxvXkPFIkQw/s1600/7sql.png" /></center></div>
