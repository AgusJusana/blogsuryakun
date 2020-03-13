+++
title = "NgeShare - Upgrade Ubuntu 12.04 ke Ubuntu 14.04"
date = 2014-04-24T12:59:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="600" data-original-width="1200" src="https://3.bp.blogspot.com/-8-E4wlwzpRE/XF3y9H2bvYI/AAAAAAAATHo/RMewvXcrlUY4-ZVFBMA06BhmrHuO2O2DQCLcBGAs/s1600/ubuntu1404.png" /></center><br />
<div style="text-align: justify;">Kali ini saya akan memberikan sebuah tutorial tentang cara untuk meng<b><i>upgrade</i></b> Ubuntu 12.04 LTS ke Ubuntu 14.04 LTS. Kebetulan tutorial ini telah saya coba tadi pagi (24/04/2014), dan alhamdulillah berhasil. So untuk kamu yang berminat dengan tutorial ini, harap diperhatikan dengan seksama, hehehe...<br /><br />
Pertama, sebelum kamu melakukan upgrade, screenshot dulu tampilan desktop Ubuntu 12.04 milikmu. Hal ini dilakukan ya itung-itung buat kenang-kenangan sama Ubuntu 12.04 karena pastinya banyak hal-hal yang udah kamu lalui bareng desktop versi itu kan. Dan juga sebagai pembanding dengan Ubuntu 14.04, hahaha... (*Ah, aneh banget nih Adminnya. -_-)<br />
<table cellpadding="0" cellspacing="0" class="tr-caption-container" style="float: left; margin-left: 0px; margin-right: 0px; text-align: left;"><tbody><tr><td style="text-align: center;"><a href="http://2.bp.blogspot.com/-O6THzN0_h0M/U1igol0eAXI/AAAAAAAAEQU/3M6uEuMh1kA/s1600/12_04.png" style="clear: left; margin-bottom: 1em; margin-left: auto; margin-right: auto;"><img border="0" src="https://2.bp.blogspot.com/-O6THzN0_h0M/U1igol0eAXI/AAAAAAAAEQU/3M6uEuMh1kA/s1600/12_04.png" /></a></td></tr><tr><td class="tr-caption" style="text-align: center;">Ubuntu 12.04</td></tr></tbody></table><br />
(*Serius lagi) Kedua, pastikan repo Ubuntu 12.04 adalah repo default Ubuntu 12.04. Kalau belum default, lokal misalnya, kamu bisa ganti repo lokal itu dengan repo default di bawah ini.<br />
<pre class="brush: js">deb http://id.archive.ubuntu.com/ubuntu/ precise main restricted universe <br />deb-src http://id.archive.ubuntu.com/ubuntu/ precise main restricted universe multiverse</pre><br />
Mengapa harus memakai repo default? Ya jawabnya simple, untuk mencegah jika terjadi kesalahan saat proses upgrade. Hal ini wajib kamu lakukan, soalnya saya pernah mencoba upgrade dengan repo lokal dan hasilnya error malahan. Buat kamu yang belum tau cara mengganti repo, bisa lihat caranya <a href="http://rezdown7.blogspot.com/2012/08/cara-mengganti-repository-ubuntu-1204.html"><b>di sini</b></a>.<br /><br />
Ketiga, setelah memastikan repo kamu sudah default, kini kamu masuk ke terminal <strike>bus</strike> (tekan CTRL+ALT+T). Masukkan perintah di bawah ini ke dalam terminal dan tekan <b>"Enter"</b>.<br />
<pre class="brush: js">sudo update-manager -d</pre><br />
Kalau sudah, akan muncul tampilan jendela <b>"Update Manager"</b>. Terlihat di situ ada tulisan <b>"New Ubuntu release '14.04' is available"</b>, dan di samping kanan tulisan tersebut ada tombol <b>"Upgrade"</b>. Langsung klik tombol <b>"Upgrade" </b>tersebut.<br />
<center><img border="0" src="https://4.bp.blogspot.com/----ObLUXiS0/U1h-l6nG0WI/AAAAAAAAEPw/zwvd9qaSGPI/s1600/2.png" /></center><br />
Keempat akan muncul tampilan seperti di bawah ini, klik <b>"Upgrade"</b>.<br />
<center><img border="0" src="https://4.bp.blogspot.com/-GH-ha5oiqV8/U1h_-VV1NEI/AAAAAAAAEP8/6RMyIAmNDuA/s1600/3.png" /></center><br />
Setelah itu, akan berlangsung proses upgrade yang cukup lama. <b><i>*Catatan, semakin banyak software yang telah kamu install di Ubuntu 12.04 milikmu, maka akan semakin lama proses upgradenya</i></b>.<br />
<center><img border="0" src="https://2.bp.blogspot.com/-rvnVJ6xLATE/U1iBGNZbuVI/AAAAAAAAEQE/qvdW1N-I1nU/s1600/4.png" /></center><br />
Tunggu hingga semua proses di atas (upgrade) selesai, hingga pada proses terakhir yaitu <b>"Restart"</b>. Selesai semua proses termasuk restart, wala....Ubuntu 12.04 milikmu kini telah sukses menjadi Ubuntu 14.04.<br />
<table cellpadding="0" cellspacing="0" class="tr-caption-container" style="float: left; margin-left: 0px; margin-right: 0px; text-align: left;"><tbody><tr><td style="text-align: center;"><img border="0" src="https://1.bp.blogspot.com/-KFfhMuUj2Uc/U1ij1QLS0gI/AAAAAAAAEQg/3IXLhb1YFmA/s1600/14_04.png" style="margin-left: auto; margin-right: auto;" /></td></tr><tr><td class="tr-caption" style="text-align: center;">Ubuntu 14.04</td></tr></tbody></table><br />
Semoga bermanfaat...<br /><br />
Oh, iya saya lupa, saya baru saja dapat bocoran tentang nama versi berikutnya dari Ubuntu, yaitu Ubuntu 14.10. Rencananya Ubuntu versi 14.10 akan diberi nama <a href="http://www.omgubuntu.co.uk/2014/04/ubuntu-14-10-name-utopic-unicorn"><b>"Utopic Unicorn"</b></a>. Ubuntu ini bukan versi LTS. Seperti apa tampilan dan pembaharuan di dalamnya? Kita tunggu di bulan Oktober (2014) mendatang.😀</div>
