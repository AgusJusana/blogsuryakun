+++
title = "NgeShare - Mengatasi Error 1935 Ketika Menginstall Microsoft Office 2016"
date = 2019-12-03T07:45:00Z
tags = ["tutorial"]
comments = true
+++

<center><img border="0" src="https://1.bp.blogspot.com/-BLoyAKh6R1M/XeM1C4k1LYI/AAAAAAAAVF8/TE6SSMoKDeIWyWAO8l65zHnvAQq2lR1wgCLcBGAsYHQ/s1600/Microsoft-Office-2016.jpg" /></center><br />
<div style="text-align: justify;">Pada kesempatan kali ini, saya ingin membagikan tutorial mengenai cara mengatasi masalah “error 1935” ketika melakukan instalasi Microsoft Office 2016. Kebetulan beberapa hari yang lalu saya sempat menemukan masalah seperti ini, tapi akhirnya dapat saya atasi setelah memperoleh solusinya dari berbagai sumber. Dan saya rasa, ada baiknya bila saya membagikan solusi tersebut, selain agar dapat membantu kawan-kawan bila nantinya menemukan masalah yang sama seperti ini, juga sebagai pengingat untuk diri saya pribadi bila mengalami kejadian semacam ini lagi (hehehe...).<br /><br />
<center><img border="0" src="https://1.bp.blogspot.com/-mMtXpw544l8/XeM0F3EHWZI/AAAAAAAAVFY/dYVLiZCBHNEM5W_nOoxZB4VdhzLOptIKwCLcBGAsYHQ/s1600/1.jpg" /></center><br />
Oiya, sebelumnya, berdasarkan dari sumber yang saya peroleh, masalah “error 1935” yang muncul ketika melakukan instalasi Ms. Office 2016 ini terjadi karena kemungkinan PC atau laptop yang akan diinstall aplikasi tersebut telah melakukan preinstalled Office 365 dari Microsoft Store yang menyebabkan error ini muncul.<br /><br />
Nah, untuk mengatasi masalah error tersebut, berdasarkan sumber yang saya peroleh adalah dengan cara menghapus terlebih dahulu key di registry PC atau laptonya, yaitu di <b>HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\AppModel\</b>. Adapun cara untuk menghapus key tersebut adalah dengan membuka aplikasi “Registry Editor”. Kamu dapat mencari aplikasi tersebut pada menu “search”.<br />
<center><img border="0" src="https://1.bp.blogspot.com/-ALtuiEfAK7E/XeMz-qDh6WI/AAAAAAAAVFU/1pf3HbEmAg4cDrjPqTE4xD7eLfJ6LzlJwCLcBGAsYHQ/s1600/2.jpg" /></center><br />
Kemudian, kamu cari key <b>HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\AppModel\</b>.<br />
<center><img border="0" src="https://1.bp.blogspot.com/-dFeNg79oMTg/XeM0L3AnTCI/AAAAAAAAVFc/en9YEZ4UGS4_P_eYYJflxszFp_12VmI1wCLcBGAsYHQ/s1600/3.jpg" /></center><br />
Lalu, hapus key tersebut.<br />
<center><img border="0" src="https://1.bp.blogspot.com/-LYQ7PwaZpxw/XeM0S9T2XeI/AAAAAAAAVFo/Kn32BSQuYBg0iNT7wLPU_ZB_rvNMprfrgCLcBGAsYHQ/s1600/4.jpg" /></center><br />
<center><img border="0" src="https://1.bp.blogspot.com/-Nl1KqLp2NOM/XeM0SRHDkpI/AAAAAAAAVFk/8hjB2eTRRBQAKc7Hr_pk36eBAb4UFsEsACLcBGAsYHQ/s1600/5.jpg" /></center><br />
Setelah kamu menghapus key tersebut, lakukanlah install ulang untuk aplikasi Microsoft Office 2016.<br />
<center><img border="0" src="https://1.bp.blogspot.com/-ACUTGVMtXuo/XeM0cX1thWI/AAAAAAAAVFw/imcH_4ML0LYsEEqdW-IYyf_cKXmr1fnFQCLcBGAsYHQ/s1600/6.jpg" /></center><br />
Oke, saya rasa itu tutorial yang dapat saya bagikan pada kesempatan kali ini. Bila ada pertanyaan ataupun saran yang terkait dengan tutorial ini, seperti biasa, saya persilahkan kawan-kawan untuk menuliskannya di kolom komentar yang berada pada tombol “Load Comments” di bawah artikel tutorial ini. Semoga tutorial ini bermanfaat ya!<br /><br /><span style="font-size: x-small;"><b>Sumber:</b><br /><a href="https://agungprasetyo.net/artikel/error-1935-ketika-instalasi-microsoft-office-2016" target="_blank">Agungprasetyo 2019</a> | <a href="https://community.spiceworks.com/topic/2156926-microsoft-office-2016-setup-failed-rolling-back-changes-windows-10" target="_blank">Spiceworks 2018</a> | <a href="https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_2016/office-2016-professional-plus-error-1935-during/63c027ab-edfb-4a0f-9fc4-4ba8bee0ad30">Microsoft 2018</a></span></div>
