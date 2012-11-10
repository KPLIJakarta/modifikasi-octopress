---
comments: true
date: 2012-09-18 07:45:34
layout: post
slug: dan-ternyata-open-jdk-aja-engga-cukup
title: 'Dan Ternyata Open JDK Aja Engga Cukup. '
wordpress_id: 291
categories:
- Android
- Java
- Linux
---

Hell yeah, android plugins buat eclipse ternyata engga mau di install open jdk di linux, muter sana - sini (halah, bahasanya) ternyata itu source repo udah diremove sama si lucid, maksud gw yang ini nich.

    deb http://archive.canonical.com/ lucid partner

Untungnya ada seseorang nan jauh di sana (halah, lagi...) menyediakan source repo ntu jdk, yach walaupun jdk 6, lumayanlah, nanti kita upgrade ya ke jdk yang baru, biar gaul gituh :D.

Ini source repo yang gw maksud

    ppa:ferramroberto/java

Gimana nambain source reponya?

    sudo add-apt-repository ppa:ferramroberto/java

Terus? biasa di update dulu, masih kaku aja :D

    sudo apt-get update

Selanjutnya di instal

    sudo apt-get install sun-java6-jdk

Udah? ya udahlah :D. Ntu source repo juga ada jre nya kalo perlu.
