+++
title = "NgeShare - Cara Menghapus Read More Otomatis di Blog"
date = 2012-09-28T16:26:00Z
tags = ["tutorial", "blogger"]
comments = true
+++

<div style="text-align: justify;"><center><img border="0" data-original-height="587" data-original-width="800" src="https://1.bp.blogspot.com/--kKTpZ2bwn8/XHMt2uV7qDI/AAAAAAAATMY/26T8EqPHbjMjVVoVWH7KaexaMbNKzyg3wCLcBGAs/s1600/read.png" /></center><br />Pada kesempatan kali ini, saya aan memberikan sebuah tips di mana tips ini tidak berkaitan dengan Linux atau Open Source melainkan berkaitan dengan blog. Tips berikut adalah tips&nbsp;<b>Cara Menghapus "Read More" Otomatis di Blog. </b>Sering kali kita jumpai tulisan&nbsp;<b>Read More/&nbsp;</b><b>Baca Selengkapnya&nbsp;</b>pada tampilan blog kita seperti di bawah ini.<br /><br />
Namun, ada kalanya kita menginginkan tulisan tersebut lenyap dari blog kita. Nah, untuk mewujudkan hal tersebut berikut ini tips dan trick yang sekiranya dapat menyelesaikan masalah Anda tersebut, mari kita simak bersama.<br /><br />
1. Langkah pertama, Login ke Akun Blogger Anda.<br />
2. Kemudian pilih Template, &nbsp;pada template Anda pilih Edit HTML &gt; Lanjutkan &gt; centang&nbsp;Expand Template Widget.<br />
3. Cari kode&nbsp;<span style="color: #0b5394;">&lt;div class='jump-link'&gt;</span> atau kode&nbsp;seperti di bawah ini, untuk lebih cepat menemukannya tekan Ctrl + F pada keyboard:<br />
<pre><code class="language-markup">&lt;b:if cond='data:blog.pageType != &amp;quot;item&amp;quot;'&gt; &lt;div class='jump-link'&gt;<br />&lt;a expr:href='data:post.url'&gt;Read more &amp;#187;&lt;/a&gt;<br />&lt;/div&gt;&lt;/b:if&gt;</code></pre><br />
4. Jika sudah ketemu, hapus kode tersebut lalu klik tombol Simpan Template.<br /><br />
Nah, readmore otomatis kini telah terhapus dari blog Anda.</div>
