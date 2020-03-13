+++
title = "NgeShare - Cara Mengalihkan Domain Lama ke Domain Baru Menggunakan Cloudflare"
date = "2020-02-26T03:35:52+07:00"
tags = ["tutorial"]
draft = false
comments = true
+++

<center><img border="0" data-original-height="675" data-original-width="1200" src="https://1.bp.blogspot.com/-PHrZvjkbB-M/XlWPUt8rUFI/AAAAAAAAVdI/L007VluKkkUQWH9ne8BTOoUxI47nkzjCwCLcBGAsYHQ/s1600/CloudFlare.jpg" /></center>
<div style="text-align: justify;">Pada kesempatan kali ini, saya ingin membagikan tutorial mengenai cara mengalihkan domain lama ke domain baru menggunakan Coudflare. Jadi, melalui tutorial ini, semisal kita memiliki sebuah website dengan domain awal/ lama, yaitu <a href="https://https://www.suryadhi.web.id/artikel/cara-mengalihkan-domain/" rel="nofollow">www.website.net</a>, lalu kita ingin membuat pengunjung yang menelusuri website dengan domain lama tersebut teralihkan secara otomatis menuju ke website dengan domain baru, yaitu <a href="https://www.suryadhi.web.id/artikel/cara-mengalihkan-domain/" rel="nofollow">www.website.com</a>, maka kita dapat melakukannya dengan menggunakan fitur <b>Page Rules</b> yang tersedia di Cloudflare. Dengan menggunakan fitur tersebut, kita tidak perlu khawatir lagi bila nantinya trafik website dengan domain baru akan anjlok dikarenakan adanya perubahan domain. Justru dengan menggunakan fitur Page Rules dari Cloudflare ini, memungkinkan trafik dari website yang berdomain baru menjadi tetap stabil karena domain lamanya masih dapat diakses oleh pengunjung dan teralihkan (redirect) secara otomatis ke domain baru.
<br/>
<br/>
Baik, daripada saya terlalu kebanyakan basa-basinya dan mungkin justru membuat bingung, langsung saja kita mulai langkah-langkah untuk menerapkannya.
<br/>
<br/>
Langkah pertama, kita buat terlebih dahulu akun <a href="https://cloudflare.com" target="_blank" rel="nofollow"><b>Cloudflare</b></a>.<br/>
<br/>
Kalau sudah selesai membuat atau memiliki akun Cloudflare, kita login menggunakan akun tersebut.<br/>
<br/>
Langkah ketiga, kita tambahkan url kedua domain website, baik yang lama maupun yang baru dengan memilih menu <b>+ Add Site</b> pada navbar Cloudflare. Oiya, setelah menambahkan url domain yang ingin dialihkan, jangan lupa untuk mengganti nameserver kedua domain yang berasal dari provider domain tersebut dengan nameserver yang telah disediakan oleh Cloudflare. Hal ini bertujuan agar domain yang kita gunakan dari provider domain dapat terhubung dengan Cloudflare.<br/>
<br/>
<center><img border="0" data-original-height="328" data-original-width="1366" src="https://1.bp.blogspot.com/-teMiPsTFuNo/XlWLyc62WtI/AAAAAAAAVck/zQ6q2lCdaeUSk4I5x0pVBWMk9PhwUSWIgCLcBGAsYHQ/s1600/5.png" /></center>
<br/>
Jika kedua domain, baik domain lama maupun domain baru telah ditambahkan ke dalam Cloudflare, maka langkah berikutnya, yaitu kita beralih ke dashboard domain lama.<br/>
<br/>
Lalu kita klik menu atau fitur <b>DNS</b>.<br/>
<br/>
Pada halaman fitur DNS, kita hapus terlebih dahulu DNS record dari provider domain. Kemudian, kita buat DNS record baru seperti di bawah ini.<br/>
<br/>
<center><img border="0" data-original-height="514" data-original-width="1366" src="https://1.bp.blogspot.com/-5RjdCvBovo0/XlWLyQULM6I/AAAAAAAAVco/Swukvsz51ekY1ml44J2d7amYKZ42aliUwCLcBGAsYHQ/s1600/6.png" /></center>
<br/>
Setelah membuat DNS record baru pada halaman fitur DNS, kita beralih ke halaman fitur <b>Page Rules</b>.<br/>
<br/>
<center><img border="0" data-original-height="615" data-original-width="1366" src="https://1.bp.blogspot.com/-15pwf_Jvruk/XlWLyeFE5_I/AAAAAAAAVcs/TbAOQ589GyAdMG-zx1Q7MfDTtAphoHHOACLcBGAsYHQ/s1600/7.png" /></center>
</br>
Pada halaman fitur Page Rules, kita buat Page Rule baru dengan mengeklik tombol <b>Create Page Rule</b>.<br/>
<br/>
<center><img border="0" data-original-height="614" data-original-width="1366" src="https://1.bp.blogspot.com/-tqpKeai9Onc/XlWLzrZkkkI/AAAAAAAAVcw/lqDd5nqsOfY8ZaQ12rDgLPZMN0ZbFJQGQCLcBGAsYHQ/s1600/8.png" /></center>
</br>
Lalu kita buat pengaturannya menjadi seperti contoh di bawah ini.<br/>
<br/>
<center><img border="0" data-original-height="591" data-original-width="1366" src="https://1.bp.blogspot.com/-LOYKO0F9oQc/XlWLz7ExsHI/AAAAAAAAVc0/KXEOo8umUXcNuSCXOYP29U3ScUhf2n8nACLcBGAsYHQ/s1600/9.png" /></center>
</br>
Setelah itu, klik tombol <b>Save and Deploy</b> dan tunggu beberapa menit.<br/>
<br/>
Langkah terakhir, kita coba menguji hasilnya.<br/>
<br/>
Kita dapat mengujinya di browser dengan mengetikkan domain lama yang akan dialihkan secara otomatis ke domain baru.<br/>
<br/>
Selain itu, kita juga dapat mengujinya dengan mengetikkan perintah <span style="background:#ddd; color:blue;padding: 0px 5px 0px 5px;">curl -I website.net</span> pada terminal yang hasilnya akan seperti contoh di bawah ini.
<pre><code class="language-markup">$ curl -I website.net
HTTP/1.1 301 Moved Permanently
Date: Wed, 26 Feb 2020 07:25:39 GMT
Connection: keep-alive
Cache-Control: max-age=3600
Expires: Wed, 26 Feb 2020 07:25:39 GMT
Location: https://www.website.com/
Server: cloudflare
CF-RAY: 55bf34872c3bv95f-ACG</code></pre>

Oke, sekiranya itu tutorial mengenai cara mengalihkan domain lama ke domain baru menggunakan Cloudflare. Bila ada pertanyaan, kritik, atau saran yang terkait dengan isi dari tutorial ini, kawan-kawan dapat menuliskannya di kolom komentar Disqus yang terletak di bawah tutorial ini. Semoga bermanfaat! 😁<br/>
<br/>
<b>Sumber:</b>
<a href="https://community.cloudflare.com/t/using-page-rules-to-perform-redirects/55386" target="_blank" rel="nofollow">Using page rules to perform redirects</a>
</div>
