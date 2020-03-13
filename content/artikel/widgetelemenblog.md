+++
title = "NgeShare - Cara Menampilkan dan Menyembunyikan Widget atau Elemen di Blog"
date = 2019-02-09T08:05:00Z
tags = ["tutorial", "blogger"]
comments = true
+++

<center><img border="0" data-original-height="600" data-original-width="1200" src="https://4.bp.blogspot.com/-CSo8SG-XlMA/XF4nJMn139I/AAAAAAAATII/wOMzR1vCMF4Vx3cjxv4a13YYRZBN41SIACLcBGAs/s1600/setting.png" /></center><br />
<div style="text-align: justify;">Buat kamu yang lagi main blog, terutama yang memakai platform dari blogger, apakah kamu pernah memiliki keinginan untuk menyembunyikan dan menampilkan widget atau elemen di blogmu. Ya, menampilkan dan menyembunyikan, seperti misalnya membuat sebuah widget atau elemen di blogmu tidak terlihat di homepage blog dan hanya dapat terlihat di postpage saja. Jika kamu memiliki keinginan seperti itu, berikut ini saya akan membagikan tutorial untuk melakukan hal tersebut dengan menggunakan beberapa kode yang dapat kamu pasang di template blogmu.<br /><br />
<b>1. Kode untuk menampilkan widget atau elemen hanya di homepage.</b><br /><pre><code><b:if cond="data:blog.url == data:blog.homepageUrl"></b:if>&lt;b:if cond='data:blog.url == data:blog.homepageUrl'&gt;<br />&lt;!-- ISI dari widget atau elemen --&gt;<br />&lt;/b:if&gt;<br /></code></pre><br />
Contoh penggunaannya:<br />
<pre><code>&lt;b:widget id='HTML1' locked='false' title='Nama title' type='HTML'&gt;<br /><span style="color: white;"><span style="background-color: #990000;">&lt;b:includable id='main'&gt;</span></span><br /><span style="color: white;"><span style="background-color: #0b5394;">&lt;b:if cond='data:blog.url == data:blog.homepageUrl'&gt;</span></span><br />&lt;!-- only display title if it's non-empty --&gt;<br />&lt;b:if cond='data:title != ""'&gt;<br />&lt;h2 class='title'&gt;&lt;data:title/&gt;&lt;/h2&gt;<br />&lt;/b:if&gt;<br />&lt;div class='widget-content'&gt;<br />&lt;data:content/&gt;<br />&lt;/div&gt;<br />&lt;b:include name='quickedit'/&gt;<br /><span style="color: white;"><span style="background-color: #0b5394;">&lt;/b:if&gt;</span></span><br /><span style="color: white;"><span style="background-color: #990000;">&lt;/b:includable&gt;</span></span><br />&lt;/b:widget&gt;<br /></code></pre><br />
Atau<br />
<pre><code><span style="color: white;"><span style="background-color: #0b5394;">&lt;b:if cond='data:blog.url == data:blog.homepageUrl'&gt;</span></span><br />&lt;style type='text/css'&gt;<br />/* -- Ini adalah CSS style -- */&lt;/style&gt;<br /><br />&lt;script type='text/javascript' &gt;<br />//Ini adalah kode JavaScript<br />&lt;/script&gt;<br /><span style="color: white;"><span style="background-color: #0b5394;">&lt;/b:if&gt;</span></span><br /></code></pre><br />
<b>Keterangan:</b><br />
- Kode yang ditandai dengan warna merah merupakan batas dari penggunaan kode tersebut.<br />
- Kode yang ditandai dengan warna biru merupakan kode untuk menampilkan atau menyembunyikan widget/ elemen.<br /><br />
<b>2. Kode untuk menampilkan widget atau elemen hanya di postpage (postingan blog)</b><code><b:if cond="data:blog.pageType == &quot;item&quot;"> </b:if></code><br />
<pre><code>&lt;b:if cond='data:blog.pageType == "item"'&gt;<br />&lt;!-- ISI dari widget atau elemen --&gt;<br />&lt;/b:if&gt;<br /></code></pre><br />
<b>3. Kode untuk menyembunyikan widget atau elemen di postpage.</b><br />
<pre><code><b:if cond="data:blog.pageType != &quot;item&quot;"></b:if>&lt;b:if cond='data:blog.pageType != "item"'&gt;<br />&lt;!-- ISI dari widget atau elemen --&gt;<br />&lt;/b:if&gt;<br /></code></pre><br />
<b>4. Kode untuk menampilkan widget atau elemen di halaman tertentu.</b><code><b:if cond="data:blog.url == &quot;URL Halaman&quot;"> </b:if></code><br />
<pre><code>&lt;b:if cond='data:blog.url == "<span style="color: white;"><span style="background-color: #0b5394;">URL Halaman</span></span>"'&gt;<br />&lt;!-- ISI dari widget atau elemen --&gt;<br />&lt;/b:if&gt;<br /></code></pre><br />
<b>Keterangan:</b><br />
- Gantilah kode yang ditandai warna biru dengan url atau link yang kamu inginkan.<br />
Contoh penggunaannya:<code><b:if cond="data:blog.url == &quot;URL Halaman&quot;"> </b:if></code><br />
<pre><code><b:if cond="data:blog.url == &quot;URL Halaman&quot;"><!-- ISI dari widget atau elemen --></b:if>&lt;b:if cond='data:blog.url == "https://suryapersonal.blogspot.com/"'&gt;<br />&lt;!-- ISI dari widget atau elemen --&gt;<br />&lt;/b:if&gt;<br /></code></pre><br />
<b>5. Kode untuk menyembunyikan widget atau elemen di halaman tertentu.</b><code><b:if cond="data:blog.url != &quot;URL Halaman&quot;"> </b:if></code><br />
<pre><code>&lt;b:if cond='data:blog.url != "<span style="color: white;"><span style="background-color: #0b5394;">URL Halaman</span></span>"'&gt;<br />&lt;!-- ISI dari widget atau elemen --&gt;<br />&lt;/b:if&gt;<br /></code></pre><br />
<b>Keterangan:</b><br />
- Gantilah kode yang ditandai warna biru dengan url atau link yang kamu inginkan.<br /><br />
<b>6. Kode untuk menampilkan widget atau elemen hanya di halaman arsip.</b><code><b:if cond="data:blog.pageType == &quot;archive&quot;"> </b:if></code><br /><pre><code>&lt;b:if cond='data:blog.pageType == "archive"'&gt;<br />&lt;!-- ISI dari widget atau elemen --&gt;<br />&lt;/b:if&gt;<br /></code></pre><br />
<b>7. Kode untuk menyembunyikan widget atau elemen di halaman arsip.</b><code><b:if cond="data:blog.pageType != &quot;archive&quot;"> </b:if></code><br /><pre><code>&lt;b:if cond='data:blog.pageType != "archive"'&gt;<br />&lt;!-- ISI dari widget atau elemen --&gt;<br />&lt;/b:if&gt;<br /></code></pre><br />
<b>8. Kode untuk menampilkan widget atau elemen hanya di halaman statis.</b><code><b:if cond="data:blog.pageType == &quot;static_page&quot;"> </b:if></code><br /><pre><code><b:if cond="data:blog.pageType == &quot;static_page&quot;"><!-- ISI dari widget atau elemen --></b:if>&lt;b:if cond='data:blog.pageType == "static_page"'&gt;<br />&lt;!-- ISI dari widget atau elemen --&gt;<br />&lt;/b:if&gt;<br /></code></pre><br />
9. Kode untuk menyembunyikan widget atau elemen di halaman statis. </b><br /><pre><code><b:if cond="data:blog.pageType != &quot;static_page&quot;">&lt;b:if cond='data:blog.pageType != "static_page"'&gt;<br />&lt;!-- ISI dari widget atau elemen --&gt;<br />&lt;/b:if&gt;</b:if><br /></code></pre><br /><b>10. Kode untuk menyembunyikan widget atau elemen di tampilan mobile.</b><br /><pre><code><b:if cond="data:blog.pageType != &quot;static_page&quot;">&lt;b:if cond='data:blog.isMobileRequest == "false"'&gt;<br />&lt;!-- ISI dari widget atau elemen --&gt;<br />&lt;/b:if&gt;</b:if><br /></code></pre><br />Oke, sekiranya itu tutorial yang bisa saya bagikan mengenai cara menampilkan dan menyembunyikan widget atau elemen di blog. Seperti biasa, kalau ada pertanyaan atau saran yang ingin kamu sampaikan terkait tutorial ini, bisa kamu sampaikan dengan cara menuliskannya di kolom komentar disqus yang terletak di bawah artikel ini. Semoga bermanfaat, ya! 😁</div>
