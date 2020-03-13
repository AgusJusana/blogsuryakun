+++
title = "NgeShare - Cara Membatasi Seleksi Teks di Artikel Web/ Blog"
date = "2020-01-23T11:36:26+07:00"
draft = false
tags = ["tutorial", "blogger"]
comments = true
+++

<div style="text-align: justify;">Pada kesempatan kali ini, saya ingin membagikan tutorial mengenai cara membatasi seleksi teks di artikel web atau blog. Jadi, melalui tutorial ini nantinya kita buat visitor yang mungkin ingin mengcopy paste isi dari artikel web/ blog hanya dapat menyeleksi teks tertentu saja. Baik, untuk tutorialnya, pertama pasang kode script di bawah ini.<br />
<pre><code class="language-css">-webkit-touch-callout:none;
-khtml-user-select:none;
-webkit-user-select:none;
-moz-user-select:none;
-ms-user-select:none;</code></pre>
</br>
Pasang kode script tersebut ke dalam elemen "post" yang ada di html template web/ blog. Untuk contoh pemasangannya seperti di bawah ini.<br />
<pre><code class="language-css">.post {
-webkit-touch-callout:none;
-khtml-user-select:none;
-webkit-user-select:none;
-moz-user-select:none;
-ms-user-select:none;
}</code></pre>
</br>
Oke, setelah selesai memasang kode script di atas, maka isi dari artikel web/ blog tidak dapat diseleksi oleh visitor.<br />
</br>
Jika ingin memberi akses kepada visitor agar dapat menyeleksi teks tertentu yang ada di dalam artikel, seperti misalnya "blockquote", "post code", atau "post pre", maka dapat menggunakan kode script di bawah ini.<br />
<pre><code class="language-css">-webkit-touch-callout:text;
  -khtml-user-select:text;
  -webkit-user-select:text;
  -moz-user-select:text;
  -ms-user-select:text;</code></pre>
</br>
Untuk pemasangannya, letakkan kode script tersebut ke dalam elemen "blockquote", "post code", atau "post pre" pada template web/ blog. Contoh pemasangannya seperti di bawah ini.<br />
<pre><code class="language-css">.post blockquote,.post pre,.post code{
  -webkit-touch-callout:text;
  -khtml-user-select:text;
  -webkit-user-select:text;
  -moz-user-select:text;
  -ms-user-select:text;
}</code></pre>
</br>
Yak, sekiranya itu tutorial mengenai cara membatasi seleksi teks di artikel web/ blog. Jika ada pertanyaan ataupun saran yang terkait dengan tutorial ini, kamu dapat menuliskannya di kolom komentar disqus yang terletak di bawah artikel ini. Semoga bermanfaat, ya! 😁</div>
