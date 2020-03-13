+++
title = "NgeShare - Cara Install VirtualBox 4.1.20 di Ubuntu"
date = 2012-08-25T06:09:00Z
tags = ["tutorial", "linux"]
comments = true
+++

<center><img border="0" src="https://3.bp.blogspot.com/-IA7Xl_-hm9A/UDgJeP8kueI/AAAAAAAACd4/ZyBRp62onJ8/s1600/virtualbox_200x175.png" /></center><br />
<div style="text-align: justify;">Beberapa waktu yang lalu, VirtualBox telah hadir dalam versi terbarunya, yaitu VirtualBox 4.1.20. Oracle, yaitu perusahaan yang merilis VirtualBox mengatakan bahwa rilisan kali ini merupakan rilis pemeliharaan terjadwal yang dirancang untuk meningkatkan stabilitas, itu tersedia untuk semua platform yang didukung.<br /><br />
<b>Apa yang baru di virtualbox 4.1.20?</b><br />
<ul><li>VMM: crash tetap dalam keadaan langka untuk VMs berjalan tanpa virtualisasi hardware</li><li>VMM: fixed analisis kode bug untuk instruksi perpindahan tertentu untuk VMs berjalan tanpa virtualisasi hardware</li><li>VMM: fixed bug interpretion untuk TPR membaca instruksi dalam kondisi langka (AMD-V saja)</li><li>Snapshots: tetap crash ketika mengembalikan sebuah snapshot tua ketika mematikan VM (bug # 9604, # 10491)</li><li>VBoxSVC: lebih toleran terhadap variabel lingkungan dengan pengkodean aneh (bug # 8780)</li><li>VGA: tetap memeriksa akses yang salah yang mungkin menyebabkan kecelakaan dalam kondisi tertentu</li><li>NAT: memperbaiki akhir untuk crash dalam kondisi langka (bug # 10.513)</li><li>Virtio-net: fixed masalah dengan penerimaan paket di GSO tamu Windows XP menyebabkan hilangnya paket di host-to-VM transfer</li><li>HPET: beberapa perbaikan (bug # 10170, # 10306)</li><li>Clipboard: menonaktifkan clipboard secara default untuk baru VMs</li><li>BIOS: BIOS PCI tidak benar terdeteksi dengan set jenis chipset untuk ICH9 (bug # 9301, # 10327)</li><li>Mac OS X host: adaptasi ke Mountain Lion</li><li>Linux Installer: perbaikan untuk Gentoo Linux (bug # 10.642)</li><li>Linux tamu: mouse integrasi tetap pada Fedora 17 tamu (bug # 2306)</li><li>Linux Penambahan: kompilasi perbaikan untuk RHEL / CentOS 6.3 (bug # 10756)</li><li>Linux Penambahan: kompilasi perbaikan untuk Linux 3.5-RC1 dan Linux 3.6-RC1 (bug # 10709)</li><li>Solaris host: tetap meditasi guru sementara mengalokasikan halaman besar (bug # 10600)</li><li>Host Solaris: fixed panik kernel mungkin sambil membebaskan memori</li><li>Solaris Installer: icon hilang tetap untuk cara pintas menu dan desktop</li></ul><br />
<b>Instal VirtualBox 4.1.20 di Ubuntu</b><br />
Buka terminal dan jalankan perintah berikut:<br />
<pre><code>gksudo gedit /etc/apt/sources.list</code></pre><br />
Anda perlu mengedit&nbsp;/etc/apt/sources.list<br /><br />Anda tambahkan baris berikut:<br />
<pre><code>deb http://download.virtualbox.org/virtualbox/debian precise contrib</code></pre><br />
Jika Anda menjalankan ubuntu 11.10 tambahkan baris berikut:<br />
<pre><code>deb http://download.virtualbox.org/virtualbox/debian oneiric contrib</code></pre><br />
Simpan File dan lalu keluar.<br /><br />
Sekarang instal PGP key menggunakan perintah berikut:<br />
<pre><code>wget -q http://download.virtualbox.org/virtualbox/debian/oracle_vbox.asc -O- | sudo apt-key add -<br /></code></pre><br />
Update source list<br />
<pre><code>sudo apt-get update<br /></code></pre><br />
Install virtualbox<br />
<pre><code>sudo apt-get install virtualbox-4.1</code></pre><br />
Jika Anda memiliki masalah dengan PPA di atas Anda dapat menngunduh paket deb <a href="https://www.virtualbox.org/wiki/Linux_Downloads"><b><span style="color: #0b5394;">di sini</span></b></a>. Once Anda memiliki paket deb yang dapat diklik dua kali di atasnya untuk menginstal paket ini.</div>
