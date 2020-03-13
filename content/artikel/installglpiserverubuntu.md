+++
title = "NgeShare - Install GLPI di Server Ubuntu 12.04"
date = 2012-09-13T12:11:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="600" data-original-width="1200" src="https://1.bp.blogspot.com/-yNMsDn1VcLk/XF5NhlNcpKI/AAAAAAAATJI/Q_n3nV2GrEQfz3TWni7GTftJNZpF49v5wCLcBGAs/s1600/glpi.png" /></center><br />
<div style="text-align: justify;">GLPI singkatan dari "Gestionnaire libre de parc informatique", GLPI adalah Sumber Daya Information Manager dengan tambahan Administrasi-Interface. Anda dapat menggunakannya untuk membangun database dengan inventarisasi untuk perusahaan Anda (komputer, software, printer ...).<br /><br />
GLPI memiliki fungsi yang disempurnakan untuk membuat kehidupan sehari-hari bagi administrator lebih mudah, seperti sistem kerja pelacakan dengan surat-pemberitahuan dan metode untuk membangun sebuah database dengan informasi dasar tentang topologi jaringan-Anda.<br /><br />
<b>Instal GLPI di Server Ubuntu 12.04</b><br />
Pertama, Anda perlu memastikan bahwa Anda memiliki ubuntu 12.04 server LAMP diinstal. Sekarang Anda perlu menginstal GLPI menggunakan perintah berikut:<br />
<pre><code>sudo apt-get install glpi<br /></code></pre><br />
Ini akan memulai instalasi, pada saat instalasi GLPI memberikan bagaimana Anda dapat mengakses setelah instalasi.<br />
<center><img border="0" src="https://3.bp.blogspot.com/-v13cQ0umWtw/UFFn4saB8TI/AAAAAAAADDI/Psd918U7GiQ/s1600/16.png" /></center><br />
GLPI konfigurasi menyediakan database untuk aplikasi ini, pilih ya dan preed masuk.<br />
<center><img border="0" src="https://1.bp.blogspot.com/-AuAlxAeU6ys/UFFn6kwtO6I/AAAAAAAADDQ/2u50qmR6bPs/s1600/25.png" /></center><br />
Memberikan password dari pengguna database admin.<br />
<center><img border="0" src="https://1.bp.blogspot.com/-TnVnvZHdYrw/UFFn-ufJI8I/AAAAAAAADDY/XNt44cTwZZo/s1600/34.png" /></center><br />
Mysql password untuk GLPI.<br />
<center><img border="0" src="https://4.bp.blogspot.com/-UT_byLeHHb8/UFFoAZjHZqI/AAAAAAAADDg/eiGX8i-44KY/s1600/41.png" /></center><br />
Konfirmasi Mysql password untuk GLPI<br />
<center><img border="0" src="https://1.bp.blogspot.com/-ASYtUZjJF-4/UFFoCLCOb7I/AAAAAAAADDo/SR_xNp7KMGQ/s1600/5.png" /></center><br />
Sekarang Anda harus mengunjungi http://ubuntu-serverip/glpi dan Anda akan melihat mirip dengan layar berikut:<br />
<center><img border="0" src="https://1.bp.blogspot.com/-YBD2y96lKPA/UFFoEsDIlDI/AAAAAAAADDw/XfNnNBsiBTo/s1600/6.png" /></center><br />
Secara default GLPI adalah memiliki username dan password berikut untuk login.<br />
<pre><code>glpi/glpi for the administrator account<br /><br />tech/tech for the technician account<br /><br />normal for the normal account<br /><br />post-only/post-only for the postonly account</code></pre><br />
Pilih nama pengguna GLPI dan password untuk login ke dalam GLPI dengan hak akses administrator dan Anda akan melihat layar berikut.<br />
<center><img border="0" src="https://3.bp.blogspot.com/-7VakrB4Fkv4/UFFpiSHLowI/AAAAAAAADD4/b7qeO-AovnQ/s1600/7.png" /></center></div>
