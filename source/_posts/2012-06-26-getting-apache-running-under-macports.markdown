---
comments: true
date: 2012-06-26 08:17:08
layout: post
slug: getting-apache-running-under-macports
title: Getting Apache Running under MacPorts.
wordpress_id: 118
categories:
- Macinthos
---

Kenapa engga nginstall xampp for mac aja?



	
  1. I used to be a linux user, using command line to install & configure all application that i need specially for my development need, yeah, i miss to interact with my terminal as i'm using linux before.

	
  2. Lama-lama bosen juga setiap kali mau "start-stop-restart" apache and mysql service mesti masukin password terus

	
  3. Automatic login ke phpmyadmin via localhost using xampp is sometime not secure walau cuma dikomputer lokal/pribadi

	
  4. Custom configuration, saya bisa semaunya nentuin path to document root buat file-file web app saya :D

	
  5. Kadang saya mesti nge-dump database yang gede-gede, dan import via phpmyadmin bawaan xampp itu kaya lagi tidur pules tiba-tiba disiram pake aer :D alias ga nyaman bgt

	
  6. DLL, kalo alesannya kurang masuk akal ya mohon dimaklumi :D, tapi kalo ada yang alesannya hampir sama seperti saya di atas, mungkin bisa menyimak tutorial di bawah ini :D


Sesuai judul yang bakal di install adalah apache untuk web server, artikel selanjutnya akan membahas mysql buat databasenya dan php buat development scriptnya, via macports. Informasi soal macports sebelumnya bisa dilihat [di sini](http://passionfactory.wordpress.com/2012/06/23/mengenal-macports-pada-mac-os-x/).

**instalasi dan konfigurasi apache via macports**



	
  1. login sebagai root kemudian install apache dengan command - _port install apache2_. Untuk mengaktifkan apache secara otomatis setiap kali komputer booting gunakan command - _port load apache2._

	
  2. Merubah directory default document root apache yang secara default berada pada directory /opt/local/apache2/htdocs, saya akan meletakan directory document root saya di /Users/nama_user_saya/Public/ biar gampang di edit :D. Edit file - _/opt/local/apache2/conf/httpd.conf  _mengunakan editor kesayangan anda, terserah mau pake nano-vim ato emacs, kemudian rubah path document root yang sebelumnya pada _/opt/local/apache2/htdocs_ ke lokasi yang diinginkan. Kemudian rubah juga pada kata <directory> sesuai dengan path dokument yang ada rubah tadi, simpan kemudian restart service apache dengan command -  _/opt/local/apache2/bin/apachectl -k restart_

	
  3. Buka browser kesayangan anda kemudian ketikan "localhost" pada browser url, kalo tampilannya seperti dibawah ini, itu artinya service apache sudah berjalan dan siap digunakan :D


[![](http://passionfactory.files.wordpress.com/2012/06/by-default-2012-06-26-at-8-05-26-am.png)](http://passionfactory.files.wordpress.com/2012/06/by-default-2012-06-26-at-8-05-26-am.png)

Untuk mencoba directory document root yang sudah dirubah tadi, saya membuat sebuah file html yang saya beri nama index.html seperti dibawah ini.

_<html><body><h1>Sudah Bisa, Alhamdulilah Ya</h1></body></html>_

Terlebih dahulu buat directory untuk file html atau file aplikasi web yang akan digunakan dengan command - mkdir  /Users/passionfactory/Public/coba. coba merupakan nama directory yang saya gunakan untuk meletakan file index.html yang saya buat tadi, kemudian sya melakukan pengujian file html yang telah saya buat tadi dengan mengetikan path file tersebut pada browser kembali. Hasil akhirnya akan seperti dibawah ini.

[![](http://passionfactory.files.wordpress.com/2012/06/by-default-2012-06-26-at-8-16-22-am.png)](http://passionfactory.files.wordpress.com/2012/06/by-default-2012-06-26-at-8-16-22-am.png)
