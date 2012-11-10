---
comments: true
date: 2012-09-19 16:16:54
layout: post
slug: namebench-untuk-internet-experience-yang-lebih-baik
title: NameBench - Untuk Internet Experience Yang Lebih Baik.
wordpress_id: 293
categories:
- Linux
---

Apaan sich?

    
    Open-source DNS Benchmark Utility. Sebuah alternatif 
    DNS Jumper diWindows dengan 100% fungsi yang sama, 
    dan tentu saja, OPEN SOURCE


Fungsinya apaan sich?

    
    Ya sama kaya DNS Jumper yang ada di Windows, untuk "mencari" DNS 
    terbaik bagi komputer kamu untuk digunakan, salah satunya untuk 
    internetan. Secara default kan akses internet kamu biasanya 
    menggunakan DNS default setiap provider. Dengan NameBench, kamu 
    bisa menggunakan alternatif DNS dengan respon terbaik, 
    bagi akses internet kamu misalnya.


Unduh dulu gan

    wget http://namebench.googlecode.com/files/namebench-1.3.1-source.tgz

Masuk ke direktori downloadan di home direktori terus Extract gan

    tar xzvf namebench-1.3.1-source.tgz

Cara menggunakan dengan command line

    #masuk ke direktorinya dulu ya ./namebench.py

Cara menggunakan dengan GUI? instal dulu gan library nya

    apt-get install python-tk

Terus?

    #masuk ke direktorinya dulu ya ./namebench.py

lah? kalo library python-tk nya udah keinstal, otomotis ngebuka gui interface pake perintah di atas, terus gimana kalo mau pake command line? --> biar keliatan hacker :D

    ./namebench.py -x
