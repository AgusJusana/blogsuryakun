+++
title = "NgeShare - Membuat Sticky Sidebar di Blog Menggunakan CSS"
date = 2019-09-13T09:52:00Z
tags = ["tutorial", "blogger"]
comments = true
+++

<center><img border="0" data-original-height="600" data-original-width="1200" src="https://1.bp.blogspot.com/-jHkg8GONMi4/XZFEsDu1wMI/AAAAAAAAUgM/-mM6NQRZnbw1d0NHX1D5-OJ9UTozWHGmACLcBGAsYHQ/s1600/sticky-sidebar.jpg" /></center><br />
<div style="text-align: justify;">Hmmm...rasa-rasanya sudah cukup lama saya tidak menuliskan sesuatu di blog ini. Yah, mohon maklum, karena rutinitas sebagai seorang freelancer sekaligus jobseeker, membuat saya sejenak vakum dari blog ini (ceileh). Namun, mumpung hari ini sedang tidak ada deadline maupun jadwal wawancara kerja, dan juga ada sedikit bahan untuk ditulis, maka saya menyempatkan waktu untuk mengupdate artikel di blog ini.<br /><br />
Oke, jadi, pada kesempatan kali ini, saya mengupdate artikel di blog ini dengan topik, yaitu tutorial “Cara Membuat Sticky Sidebar di Blog Menggunakan CSS” tanpa javascript. Bagi kamu yang seorang blogger dan mungkin sedang ingin mencustom atau mempercantik tampilan blogmu, saya rasa tutorial kali ini akan dapat membantu keinginanmu tersebut.<br /><br />
Oh, iya, ngomong-ngomong soal “Sticky Sidebar”, sebenarnya apa sih itu? Mungkin di antara kamu ada yang bingung dengan istilah tersebut. Oke, saya jelaskan secara singkat ya. Sticky Sidebar adalah elemen sidebar dalam sebuah template blog yang memiliki posisi tetap (statis) ketika suatu halaman blog atau web sedang discroll (diarahkan) ke bawah. Jadi, dengan membuat sticky sidebar ini, nantinya widget blogmu yang terpasang di elemen sidebar akan memiliki posisi yang tetap dan mengikuti arah scroll. Untuk gambaran lebih jelasnya mengenai sticky sidebar, dapat kamu lihat dengan menekan tombol “Result” di bawah ini.<br /><br />
<center><div style="text-align: center;"><ul class="button"><li><a class="demo" href="https://codepen.io/suryacodekun/pen/oNvywBy" rel="nofollow noopener" target="_blank">Result</a></li></ul></div></center><br /><br />
Baik, tanpa perlu basa-basi lagi, mari simak tutorial cara pembuatannya yang mudah dan singkat di bawah ini.<span style="font-size: large;"><b>&nbsp;</b></span><br /><br /><span style="font-size: large;"><b>Cara Membuat Sticky Sidebar di Blog Menggunakan CSS</b></span><br /><br />1. Langkah pertama, copy kode di bawah ini.<br />
<pre><code class="language-css">position: -webkit-sticky;<br />position: sticky;<br />top: 10px;</code></pre><br />
2. Kemudian, letakkan atau pastekan kode tersebut ke dalam elemen sidebar blogmu.<br /><br />Contoh pemasangannya adalah seperti berikut ini:<br />
<pre><code class="language-css">#sidebar-wrapper {<br />width: 100%;<br />max-width: 300px;<br />padding: 20px 5px 5px 5px;<br />float: right;<br />margin: 0 auto;<br />position: -webkit-sticky;<br />position: sticky;<br />top: 10px;<br />}</code></pre><br />
3. Nah, setelah itu, jangan lupa simpan perubahan yang telah kamu terapkan di template blogmu. Lalu lihat hasilnya.<br /><br />Mudah, bukan? Hehehe...<br /><br />
Oke, sekiranya itu tutorial yang dapat saya bagikan kali ini. Jika kamu memiliki saran atau pertanyaan yang terkait dengan artikel tutorial ini, kamu dapat menyampaikannya dengan menuliskannya di kolom komentar blog ini dengan menekan tombol “Load Comments” yang terletak di bawah artikel ini. Semoga bermanfaat, ya!</div>
