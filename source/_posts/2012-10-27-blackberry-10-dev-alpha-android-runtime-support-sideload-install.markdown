---
comments: true
date: 2012-10-27 23:18:01
layout: post
slug: blackberry-10-dev-alpha-android-runtime-support-sideload-install
title: Blackberry 10 Dev Alpha, Android Runtime Support & Sideload Install.
wordpress_id: 351
categories:
- Android
- Dear Diary
- Java
- Macinthos
---

Pada event Blackberry 10 Jam World Tour Jakarta, saya bersama beberapa peserta terpilih berkesempatan untuk mendapatkan prototype blackberry 10 yang dinamakan blackberry 10 dev alpha. Sebenarnya ini bukan berita baru, tetapi karena baru belakangan ini saya bisa hands-on dengan prototype blackberry 10 tersebut, dan menemukan beberapa hal menarik, salah satunya adalah mengenai metode pengembangan baru menggunakan android runtime, yang dalam hal ini menguntungkan developer yang mengembangkan aplikasi android untuk melakukan porting dengan mudah pada device blackberry 10 nantinya ketika sudah resmi di launching.

Tujuan RIM membagikan prototype blackberry 10 tersebut kepada developer tidak lain adalah untuk memberikan kesempatan kepada developer baik yang berbasis native development (QT, C++), webwork, air dan android runtime untuk mencoba mengembangkan aplikasi di blackberry 10, saya sendiri karena memiliki latar belakang pengembangan berbasis android, mencoba untuk menggunakan metode berbasis android runtime, melakukan porting aplikasi yang pernah saya buat menggunakan tool yang sudah disediakan resource nya di [sini](http://developer.blackberry.com). Menarik, bahkan dengan online tool yang tersedia, saya tidak perlu melakukan perubahan sama sekali pada kode program android yang pernah saya buat, saya hanya perlu mengimport .apk saya dan secara otomatis online tool tersebut akan melakukan konversi menjadi .bar yang merupakan format file aplikasi yang juga merupakan format file aplikasi pada playbook.

Saya tidak akan menyinggung banyak mengenai blackberry 10 dev alphanya, secara berkala saya akan mencatat hands-on saya di blog ini mengenai blackberry 10 dev alpha tersebut, yang akan saya sampaikan selanjutnya adalah mengenai metode instalasi aplikasi yang sudah saya porting (tanpa menemui kendala / tidak gagal) juga beberapa aplikasi android (yang free tentunya) yang sengaja saya coba porting untuk saya gunakan pada blackberry 10 dev alpha ini, karena saya terkesan dengan user interface dan experiencenya.

Metode instalasi yang saya gunakan dinamakan sideload, dimana saya akan menginstalasikan secara langsung melalui jaringan wifi yang terhubung pada network yang sama menggunakan playbook tools yang bisa di download [di sini](http://www.mediafire.com/?msi5u4ni3h8nx53). Saya menggunakan OS X, dan belum mencoba metode ini pada Windows, setelah di download extract file playbook tools yang sudah di download pada direktori yang anda inginkan. Berikut ini beberapa tahap yang dilakukan :



	
  1. Pastikan mengetahui ip address yang digunakan oleh blackberry 10 dev alpha dengan membuka menu setting - network connections - wifi - advanced - internet connection yang akan digunakan pada proses instalasi.

	
  2. Aktifkan development mode yang terdapat pada menu setting - security and privacy - development mode, masukan password yang akan digunakan pada proses instalasi nantinya

	
  3. Letakan aplikasi android yang sudah diporting (.bar) pada kedalam direktori yang sama dengan file playbook tool yang sudah di extract kemudian gunakan perintah dibawah ini untuk melakukan instalasi menggunakan metode sideload, sebagai contoh saya akan melakukan instalasi twitter for android yang sudah diporting menjadi file .bar


    java -Xmx512M -jar BarDeploy.jar -installApp -device 192.168.1.101 -password 1234 Twitter.bar

sesuaikan dengan ip address dan password development mode pada device, serta nama aplikasi yang diinstalasikan. Menarik bukan, bisa menggunakan aplikasi android yang biasa digunakan + BBM-an, seperti memiliki android device dan blackberry dalam 1 device, thats all :-)
