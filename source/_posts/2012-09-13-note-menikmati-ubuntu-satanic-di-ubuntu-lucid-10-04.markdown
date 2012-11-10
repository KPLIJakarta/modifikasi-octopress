---
comments: true
date: 2012-09-13 05:29:14
layout: post
slug: note-menikmati-ubuntu-satanic-di-ubuntu-lucid-10-04
title: '[Note] Menikmati Ubuntu Satanic di Ubuntu Lucid 10.04'
wordpress_id: 257
categories:
- Linux
---

Download Secure Key Repository

    
    wget -q http://ubuntusatanic.org/ubuntu-se-key.gpg -O- 
    | sudo apt-key add -


Edit Source Repository

    
    vim etc/apt/sources.list


Tambahkan Source Repository Ubuntu Satanic

    
    deb http://ubuntusatanic.org/hell oneiric main


Update Source Repository

    
    apt-get update


Instal Ubuntu Satanic Package

    
    apt-get install ubuntu-satanic-wide


Menggunakan Desktop Wallpaper Ubuntu Satanic

    
    Klik kanan desktop - Change desktop background - Background


Menggunakan Ubuntu Satanic Theme

    
    Klik kanan desktop - Change Desktop Background - Theme


Menggunakan Sound Ubuntu Satanic Theme

    
    System - Preferences - Sound - Satanic


Menggunakan GDM Login Theme Ubuntu Satanic

    
    #Pada Terminal Ketik
    
    sataniconf gdm SE-Satanic


Menggunakan Plymouth Theme Ubuntu Satanic

    
    #Pada Terminal Ketik
    sataniconf plymouth satanic-logo


[![](http://passionfactory.files.wordpress.com/2012/09/screenshot1.png)](http://passionfactory.files.wordpress.com/2012/09/screenshot1.png)
