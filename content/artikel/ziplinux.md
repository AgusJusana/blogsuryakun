+++
title = "NgeShare - Cara Menggunakan Perintah Zip di Linux"
date = 2018-12-04T06:45:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" data-original-height="600" data-original-width="1200" src="https://4.bp.blogspot.com/-cm9-TvWXies/XDPs6fcH-XI/AAAAAAAASv0/5bOF7ZKLEMgGaQc5lmQlAmQRpoQlH4s4wCLcBGAs/s1600/tutorial.jpg" /></center><br />
<div style="text-align: justify;">Yosh, pada kesempatan kali ini, saya akan membagikan tutorial mengenai sebuah perintah di Linux. Perintah ini adalah "zip" yang memiliki fungsi untuk memaketkan atau meng-kompres sebuah/ beberapa file menjadi arsip file/ folder berekstensi .zip seperti contoh di bawah ini:<br />
<center><img border="0" data-original-height="410" data-original-width="700" src="https://3.bp.blogspot.com/-aBZw8MClnOs/XAWznirC32I/AAAAAAAASoU/ocDuT-yYu8c1Eb0sDiu_kHLTMGhMidCqACLcBGAs/s1600/2.jpg" /></center><br />
Ya, meskipun saat ini telah ada cara yang lebih mudah untuk meng-kompres file menjadi arsip file/ folder .zip di Linux, yaitu dengan cara klik kanan seperti di bawah ini:<br />
<center><img border="0" data-original-height="477" data-original-width="851" src="https://1.bp.blogspot.com/-xOhru25bvek/XAWzWykuEVI/AAAAAAAASoM/67FGfzXaOLoGJgiuJux3G9knCirOOlfMACLcBGAs/s1600/1.jpg" /></center><br />
Tapi, tak ada salahnya kan kalau kamu mengetahui cara/ alternatif lain untuk tetap dapat menjalankan fungsi (zip) tersebut? (Hehehe...) Alternatif lainnya seperti dengan menggunakan perintah "zip" pada terminal. Bagaimana caranya? Oke, simak tutorialnya berikut ini:<br /><br />
<span style="font-size: large;"><b>Meng-kompres Sebuah File</b></span><br />
Misalkan kamu memiliki sebuah file bernama "tes.txt" yang ingin kamu kompres menjadi "file.zip", maka kamu dapat meng-kompres file tersebut di terminal dengan menjalankan perintah:<br />
<pre class="command"><code spellcheck="false">zip file.zip tes.txt</code></pre><br />
Kemudian tekan tombol "Enter", akan muncul pesan seperti di bawah ini setelah kamu menjalankan perintah tersebut.<br />
<pre><code spellcheck="false">adding: tes.txt (stored 0%)</code></pre><br />
Pesan ini menandakan bahwa file "tes.txt" tadi telah berhasil terkompres menjadi "file.zip".<br /><br />
<span style="font-size: large;"><b>Meng-kompres Beberapa File</b></span><br />
Misalkan kamu memiliki beberapa file yang bernama "tes1.txt", "tes2.txt", "tes3.txt", dan "tes4.txt", dan kamu ingin meng-kompres file-file tersebut ke dalam sebuah arsip file bernama "files.zip", maka kamu dapat melakukannya dengan menjalakan perintah seperti berikut ini di terminal:<br />
<pre class="command"><code spellcheck="false">zip files.zip tes1.txt </code><code spellcheck="false">tes2.txt </code><code spellcheck="false">tes3.txt </code><code spellcheck="false">tes4.txt</code></pre><br />
Kemudian tekan tombol "Enter", akan muncul pesan seperti di bawah ini yang menandakan bahwa file-filemu tadi telah berhasil terkompres menjadi sebuah file, yaitu "files.zip".<br />
<pre><code>adding: tes1.txt (stored 0%)<br />adding: tes2.txt (stored 0%)<br />adding: tes3.txt (stored 0%)<br />adding: tes4.txt (stored 0%)</code></pre><br />
<span style="font-size: large;"><b>Meng-kompres Folder</b></span><br />
Misalkan kamu memiliki folder bernama "files", dan kamu ingin meng-kompresnya&nbsp; "files.zip", maka  kamu dapat melakukannya dengan menjalakan perintah:<br />
<pre class="command"><code spellcheck="false">zip files.zip files</code></pre><br />
Kemudian tekan tombol "Enter", akan muncul pesan seperti di bawah ini  yang menandakan bahwa folder tadi telah berhasil terkompres menjadi "files.zip".<br /><pre><code spellcheck="false">adding: files/ (stored 0%)</code></pre><br />
<span style="font-size: large;"><b>Menghapus File dari Arsip File/ Folder Zip</b></span><br />
Kalau misalnya kamu ingin menghapus file "tes1.txt" dari arsip "files.zip", maka kamu harus menjalankan perintah:<br /><pre class="command"><code spellcheck="false">zip -d files.zip tes1.txt</code></pre><br />
Setelah itu akan muncul pesan seperti di bawah ini yang menandakan bahwa file "tes1.txt" tadi telah terhapus.<br /><pre><code spellcheck="false">deleting: tes1.txt</code></pre><br />
<span style="font-size: large;"><b>Menambahkan Beberapa File ke Dalam Arsip File/ Folder Zip</b></span><br />
Ketika kamu ingin menambahkan beberapa file seperti misalnya file "tes5.txt" dan "tes6.txt" ke dalam arsip file/ folder "files.zip", kamu dapat melakukannya dengan menjalankan perintah seperti berikut ini:<br /><pre class="command"><code spellcheck="false">zip -u files.zip tes5.txt tes6.txt</code></pre><br />
Setelah itu akan muncul pesan seperti di bawah ini yang menandakan bahwa file "tes5.txt" dan "tes6.txt" tadi telah berhasil ditambahkan ke dalam arsip "files.zip".<br /><pre><code spellcheck="false">adding: tes5.txt (stored 0%)<br />adding: </code><code spellcheck="false"><code spellcheck="false">tes6</code>.txt (stored 0%)</code></pre><br />
Oke, sekiranya itu tutorial mengenai cara menggunakan perintah zip di linux. Seperti biasa, kalau ada pertanyaan atau saran yang ingin kamu sampaikan kepada saya, kamu dapat menuliskannya pada kolom komentar yang letaknya ada di bawah postingan ini.<br /><br />
Semoga bermanfaat ya! 😊</div>
