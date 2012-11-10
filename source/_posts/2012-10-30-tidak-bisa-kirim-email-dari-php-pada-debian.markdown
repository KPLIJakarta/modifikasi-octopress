---
comments: true
date: 2012-10-30 16:53:26
layout: post
slug: tidak-bisa-kirim-email-dari-php-pada-debian
title: Tidak Bisa Kirim Email Dari PHP Pada Debian?
wordpress_id: 362
categories:
- Linux
---

Oke, intinya engga bisa ngirim email verifikasi abis ngisi sign in form, tanya kenapa?

    
    1. Kebiasaan pake hostingan and tinggal terima beres konfigurasi server
    2. Sekarang ceritanya ngelola server sendiri, and baru sadar email verifikasinya engga bisa terkirim


And here's the info

    
    1. Debian 6
    2. PHP5
    3. Just web server, so you need to install mail transfer agent (MTA)
    4. you need to know your server ip and hostname


How to solve?

    
    /* Instal exim untuk MTA */
    
    apt-get install exim4-daemon-light
    
    /* Konfigurasi */
    
    dpkg-reconfigure exim4-config


Terus?

    
    Jawab pertanyaan yang ada? ciyus? miapah? :D
    
    General type of mail configuration: internet site; mail is sent and received directly using SMTP
    System mail name: (this should be your servers full hostname) #isi hostname server
    IP-addresses to listen on for incoming SMTP connections:127.0.0.1;isi_ip_server
    Other destinations for which mail is accepted: Select ok
    Domains to relay mail for: blank, select ok
    Machines to relay mail for: blank, select ok
    Keep number of DNS-queries minimal (Dial-on-Demand)? No
    Delivery method for local mail: mbox format in /var/mail/
    Split configuration into small files? Yes
    Root and postmaster mail recipient: isi dengan lokal user server


Selesai, coba kirim email dari script php kamu :-)
