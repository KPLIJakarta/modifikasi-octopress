---
comments: true
date: 2012-06-23 08:18:33
layout: post
slug: mengenal-macports-pada-mac-os-x
title: Mengenal MacPorts Pada Mac OS X.
wordpress_id: 111
categories:
- Macinthos
---

MacPorts, sebelumnya dikenal sebagai DarwinPorts merupakan sebuah manajeman perangkat lunak yang memudahkan instalasi aplikasi pada sistem operasi macinthos. Umumnya perangkat lunak yang diinstalasikan melalui macport merupakan aplikasi open source. Manajemen perangkat lunak ini memiliki kesamaan tujuan dan fungsi seperti yang terdapat pada keluarga port BSD, apt-get pada Debian dan turunannya, yaitu untuk memudahkan instalasi paket instalasi dengan memenuhi setiap depedensi yang dibutuhkan oleh setiap paket aplikasi yang diinstal secara otomatis. Perintah sederhana yang digunakan untuk menggunakan macports adalah _#port install <nama aplikasi>_.

MacPort saat ini dihost pada Mac OS Forge, sebuah repository perangkat lunak pihak ketiga yang dibuat dan dikelola oleh perusahaan Apple. Pada Agustus 2011, MacPorts telah mencapai versi 2.0.1 dengan koleksi port sekitar 8300 buah. Kabar baiknya, mirror lokal macports kini tersedia di Indonesia, berita selengkapnya bisa di lihat di [sini](http://dailysocial.net/2011/11/23/mirror-macports-kini-tersedia-di-indonesia/).

Instalasi MacPorts.

Download dan install macports yang sesuai dengan sistem operasi anda di [sini](https://distfiles.macports.org/MacPorts/), dengan catatan aplikasi X Code developer tool telah terinstal sebelumnya, bagi pengguna Mac OS X Lion, instalasi X Code dapat dilakukan melalui App Store. Setelah X Code dan MacPorts terinstall, instalasikan komponen command line tool pada X Code dengan membuka menu X Code - preference - Download. Setelah itu buka terminal dan pastikan macports yang terintal merupakan versi terupdate dengan mengetik perintah _sudo port -v selfupdate_.

[![](http://passionfactory.files.wordpress.com/2012/06/by-default-2012-06-22-at-3-41-30-pm.png)](http://passionfactory.files.wordpress.com/2012/06/by-default-2012-06-22-at-3-41-30-pm.png)


Dibawah ini merupakan screenshoot beberapa perintah dasar untuk menggunakan macports dari situs http://developer.apple.com/.




[![](http://passionfactory.files.wordpress.com/2012/06/by-default-2012-06-23-at-8-17-16-am.png)](http://passionfactory.files.wordpress.com/2012/06/by-default-2012-06-23-at-8-17-16-am.png)
