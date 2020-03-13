+++
title = "NgeShare - Melihat History Command di Linux"
date = 2018-09-15T21:09:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="600" data-original-width="1200" src="https://1.bp.blogspot.com/-0b189IE-eNk/XDWXELCsPlI/AAAAAAAAS3Q/fghbEkX8sOgE1arYMg_U2FimhzTCcOAUwCLcBGAs/s1600/history.png" /></center><br /><div style="text-align: justify">Pada postingan kali ini, saya akan memberikan tips atau solusi kepada agan "pengguna Linux" untuk dapat melihat history command atau perintah-perintah yang telah agan jalankan di terminal selama memakai OS Linux milik agan. Tips berikut ini dapat membantu agan untuk melihat atau mengingat <strike>mantan</strike> kembali perintah-perintah tersebut. Selain itu, melalui tips ini nantinya agan dapat lebih menghemat waktu dalam mengerjakan atau menjalankan perintah pada OS Linux agan. Oh, iya, sebelumnya, tips ini telah saya coba di OS Linux Lubuntu 18.04, dan alhamdulillah berhasil. Oke, tanpa perlu panjang lebar, agan bisa menyimak tips berikut ini.<br /><br />
<b><span style="font-size: large;">1. Menjalankan perintah 'history'.</span></b><br />
Agan dapat menjalankan perintah ini dengan memasukkan perintah <span style="color: #0b5394;">history</span> pada terminal seperti tampilan di bawah ini.<br />
<center><img border="0" data-original-height="466" data-original-width="656" src="https://3.bp.blogspot.com/-CBE63v1nHF8/W50NqSK9aWI/AAAAAAAARnQ/WD1WQwBjFx49JjspE7AoVuWaskDLycsbgCLcBGAs/s1600/1.jpg" /></center><br />
Dengan menjalankan perintah <span style="color: #0b5394;">history</span> di terminal, agan akan dapat melihat beberapa perintah yang telah agan jalankan selama menggunakan OS Linux.<br />
<b><span style="font-size: large;">2. Menampilkan history command secara detail dengan tanggal dan waktu.</span></b><br />
Jika agan ingin menampilkan tanggal dan waktu ketika agan menjalankan perintah-perintah tersebut, agan dapat melakukannya dengan memasukkan perintah di bawah ini ke dalam terminal, kemudian jalankan perintah <span style="color: #0b5394;">history</span> kembali.<br />
<pre><code><br />export HISTTIMEFORMAT="%F %T: "<br /></code></pre><br />
<center><img border="0" data-original-height="466" data-original-width="656" src="https://1.bp.blogspot.com/-mx-1WYQwKNM/W50Omm__3WI/AAAAAAAARnY/1UtSUN6GmSwnxsBjfMegi2-y6NS9mBq5gCLcBGAs/s1600/2.jpg" /></center><br />
Pada tampilan di atas, agan mungkin bertanya-tanya mengapa detail tanggal dan waktu yang muncul untuk setiap perintah terlihat sama, bukankah seharusnya berbeda? Hmmm...terkait dengan masalah tersebut, terdapat penjelasan dari <a href="https://unix.stackexchange.com/questions/87740/histtimeformat-does-not-show-correct-date-and-time-for-history" target="_blank"><b>StackExchange</b></a> berikut ini yang dapat menjawab permasalahan tersebut.<br /><blockquote class="tr_bq"><i>If you set the <span style="color: #b45f06;">HISTTIMEFORMAT</span> in bash your new entries get stored in the history file with a timestamp, older commands that don't have a timestamp (those before you ever set <span style="color: #b45f06;">HISTTIMEFORMAT</span> will display one and the same date-time-stamp (I assume the one from the first entry found with a real timestamp).<br /><br />This problem should solve itself after your complete history has been updated in a few days.<br /><br />You can look in <span style="color: #b45f06;">~/.bash_history</span> to see what is the first line that has a date-time-stamp. Those are lines starting with a <span style="color: #b45f06;">#</span> followed by a (currently) 10 digit number.</i></blockquote>Oke, sekiranya itu dulu tips yang dapat saya berikan saat ini. Bila agan memiliki pertanyaan, saran ataupun masukan, agan dapat menuliskannya di kolom komentar. Terima kasih... 😊<br /><blockquote class="tr_bq">History never really says goodbye. History says, 'See you later.' <span style="color: #0b5394;"><span style="font-size: x-small;">- Eduardo Galeano</span></span></blockquote></div>