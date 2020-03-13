+++
title = "NgeShare - Coba Ubuntu WebApps"
date = 2012-08-03T16:52:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" src="https://1.bp.blogspot.com/-kz0ehuRWFm8/UBue8dSIQvI/AAAAAAAACGI/62MEQkm0Erk/s1600/ubuntuwebs.jpg" /></center><br />
<div style="text-align: justify;">Agan-agan pastinya telah mengenal apa itu Ubuntu WebApps, yah Ubuntu WebApps adalah sebuah fitur yang dibuat dan dikembangkan untuk mendukung tampilan Ubuntu 12.10 Quantal Quetzal.&nbsp;Dengan Ubuntu webapps websites seperti Gmail, Grooveshark, Last.fm, Facebook, Google Docs dan banyak lagi yang terintegrasi dengan desktop Ubuntu.<br /><br />
Webapps ini sepenuhnya terintegrasi dengan Unity HUD, Sound &amp; Messaging notifications menu dan dukungan Unity Quicklists.&nbsp;Webapps dapat digunakan dengan berbagai cara menarik, dan kemungkinan tidak terbatas. Untuk saat ini Ubuntu WebApps masih dalam tahap pengembangan dan akan dirilis secara default bersama dengan dirilisnya Ubuntu 12.10 Quantal Quetzal.<br />
<center><img border="0" data-original-height="575" data-original-width="872" src="https://3.bp.blogspot.com/-JgsYbP-bgS4/W-qvUfv7A2I/AAAAAAAASK0/0VP1lbg0V-QTfaaFxpMOOTc2QSJGlvdBQCLcBGAs/s1600/online-accounts.jpg" /></center><br />
<b>Menjajal Ubuntu WebApps</b><br />
Perlu diketahui, bahwa teknologi ini masih dalam tahap pengembangan, jadi jangan berharap banyak dan harap maklum jika masih banyak bug di sana sini. Silakan ketik perintah berikut untuk menginstalnya:<br />
<pre><code>sudo add-apt-repository ppa:webapps/preview<br />sudo apt-get update<br />sudo apt-get install unity-webapps-preview</code></pre><br />
Setelah proses instalasi selesai, silakan restart atau logout komputer kalian.<br /><br />Nah, jika sudah puas mencoba atau WebApps malah bikin error, silakan balikin lagi seperti semula dengan mengetik perintah berikut:<br />
<pre><code>sudo apt-get install ppa-purge<br />sudo ppa-purge ppa:webapps/preview<br />sudo apt-get remove gnome-control-center-signon signond signon-keyring-extension signon-plugin-oauth2 signon-ui libunity-webapps-chromium unity-chromium-extension unity-lens-gdocs unity-lens-photo unity-scope-flickr xul-ext-webaccounts xul-ext-unity xul-ext-websites-integration</code></pre></div>
