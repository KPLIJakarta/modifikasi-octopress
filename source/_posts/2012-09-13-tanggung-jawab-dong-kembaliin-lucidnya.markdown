---
comments: true
date: 2012-09-13 20:16:51
layout: post
slug: tanggung-jawab-dong-kembaliin-lucidnya
title: Tanggung - Jawab Dong, Kembaliin Lucidnya.
wordpress_id: 274
categories:
- Linux
---

Lah, katanya biar metal!!!, nyobain ubuntu satanic di lucid?. Ya sebagai sebuah pertanggung-jawaban, udah bisa "bongkar" terima "pasang" juga dong, ya wes ya wes.

Oke, kembaliin default boot nya dulu

    
    sudo update-alternatives --config default.plymouth


Ngembaliin default gdm nya

    
    cp /usr/share/applications/gnome-appearance-properties.desktop 
    /usr/share/gdm/autostart/LoginWindow/
    
    #log out, terus ganti background dan theme defaultnya 
    si lucid terus login


Menggunakan background gdm dan theme yang sudah dipilih menjadi default

    
    rm /usr/share/gdm/autostart/LoginWindow/
    gnome-appearance-properties.desktop


Rubah theme, rubah dekstop wallpaper, rubah sound jadi bawaan defaultnya si lucid, terakhir restart gnome-panelnya

    
    killall gnome-panel


Reboot buat nyoba

    
    sudo reboot
