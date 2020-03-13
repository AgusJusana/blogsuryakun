+++
title = "NgeShare - Mengatasi Error Deploy Hugo di Github"
date = "2020-01-01T04:25:06+07:00"
draft = false
tags = ["tutorial"]
comments = true
+++

<div style="text-align: justify;">Beberapa waktu yang lalu saya baru saja melakukan migrasi blog ke Hugo. Namun, setelah selesai melakukan migrasi dan ingin mengupdate konten blog, saya justru menemui masalah error seperti pada gambar di bawah ini.<br />
<center><img border="0" data-original-height="138" data-original-width="563" src="https://1.bp.blogspot.com/-QBq_rxdL3Os/Xgu62tziqCI/AAAAAAAAVPQ/u1m8bCJmIKcuCx5IHduq5TixN1W8nYZmwCLcBGAsYHQ/s1600/error.jpg" /></center>
<br />
Setelah telusuri ke sana kemari terkait masalah ini, saya menyadari bahwa ternyata hal itu terjadi karena saya belum menjalankan perintah "pull" atau "--force" terlebih dahulu sebelum menjalankan perintah deploy. Perintah "pull" atau "--force" sendiri digunakan untuk me-merge file maupun folder yang telah dirubah atau baru saja dibuat ke web hosting. Jadi, setiap kali ada pembaruan di blog hugo, diharuskan untuk me-merge file maupun folder yang diperbarui dengan perintah "pull" ataupun perintah "--force" terlebih dahulu. Kalau untuk solusi dari masalah error yang saya hadapi ini, saya menggunakan perintah "--force" seperti di bawah ini.<br />
<pre><code class="language-css">git push -u origin master --force</code></pre>
<br />
Untuk proses penerapannya sendiri, yaitu pertama buka terlebih dahulu direktori blog hugo di terminal.<br />
<pre><code class="language-css">cd blog</code></pre>
<br />
Kemudian, masuk ke direktori "public".<br />
<pre><code class="language-css">cd public</code></pre>
<br />
Pada diretori "public", masukkan perintah "--force", lalu tunggu hingga prosesnya selesai.<br /><br />
Baru setelah itu, kembali lagi ke direktori blog hugo dan jalankan proses deploy.<br />
<blockquote class="tr_bq"><b>NB:</b> Oiya, tutorial ini hanya berlaku untuk blog Hugo yang menggunakan hosting Github, ya. Kalau hosting yang digunakan berbeda, maka cara untuk mengatasi error deploynya juga akan berbeda. 😅</blockquote></div>
