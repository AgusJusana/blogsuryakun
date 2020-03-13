+++
title = "NgeShare - Cara Restore Default Lubuntu Panel"
date = 2018-09-14T06:33:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="600" data-original-width="1200" src="https://3.bp.blogspot.com/-vNXvtc8tNeI/XFzXr7ROudI/AAAAAAAATF4/jlfLHBPYq6EGfckBSTh-a8AkCk3PTA4RQCLcBGAs/s1600/restore.png" /></center><br />
<div style="text-align: justify;">Beberapa waktu yang lalu, saya merasa bosan dengan tampilan panel <a href="https://lubuntu.me/" target="_blank"><b>Lubuntu</b></a> milik saya yang telah saya custom seperti di bawah ini.<br /><br /><table align="center" cellpadding="0" cellspacing="0" class="tr-caption-container" style="margin-left: auto; margin-right: auto; text-align: center;"><tbody><tr><td style="text-align: center;"><img border="0" data-original-height="94" data-original-width="1366" src="https://2.bp.blogspot.com/-zpU7_--HdRs/W5rwpS6jKrI/AAAAAAAARmk/59A4IDKLn44oBBgjPOTmLuFvXqHXr8luQCEwYBhgL/s1600/panelcustom.jpg" /></td></tr><tr><td class="tr-caption" style="text-align: center;">Custom Panel</td></tr></tbody></table><br />
Saya merasa bosan dengan tampilan tersebut karena telah lama saya gunakan, dan muncul keinginan saya untuk menggunakan tampilan panel default Lubuntu. Untuk itu, maka saya harus mengembalikannya (restore) ke tampilan defaultnya.<br /><br />
Alhasil, saya menjalankan keinginan saya tersebut dengan mencari beberapa solusi, dan kemudian saya menemukan sebuah solusi dari <b><a href="https://askubuntu.com/questions/64631/how-to-restore-the-default-lubuntu-panel" target="_blank">askubuntu</a></b> yang berhasil mengubah panel custom saya tersebut menjadi panel default. Caranya sangat mudah sekali, cukup dengan menjalankan dua perintah di bawah ini ke dalam terminal.<br />
<pre><code>rm -r ~/.config/lxpanel</code></pre><br />
<pre><code>lxpanelctl restart</code></pre><br />
Setelah saya coba, dua perintah tersebut efektif dan bekerja di Lubuntu milik saya, tebukti dengan hasilnya yang dapat membuat tampilan panel Lubuntu milik saya kini menjadi default kembali.<br /><br /><table align="center" cellpadding="0" cellspacing="0" class="tr-caption-container" style="margin-left: auto; margin-right: auto; text-align: center;"><tbody><tr><td style="text-align: center;"><img border="0" data-original-height="76" data-original-width="1366" src="https://2.bp.blogspot.com/-LctL3znKpsc/W5ryS6lHHBI/AAAAAAAARmw/5uUHfuqqiUYWJLJgxpChonSLsvdfhNPwQCEwYBhgL/s1600/paneldefault.jpg" /></td></tr><tr><td class="tr-caption" style="text-align: center;">Default Panel</td></tr></tbody></table><br />
Jika agan ingin membuat tampilan panel Lubuntu agan menjadi default, mungkin cara di atas dapat membantu agan. Semoga sukses... 😊 </div>
