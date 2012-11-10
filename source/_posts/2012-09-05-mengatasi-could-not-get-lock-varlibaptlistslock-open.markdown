---
comments: true
date: 2012-09-05 16:48:56
layout: post
slug: mengatasi-could-not-get-lock-varlibaptlistslock-open
title: '[Mengatasi] Could not get lock /var/lib/apt/lists/lock - open.'
wordpress_id: 242
categories:
- Linux
---

Periksa, apakah aplikasi yang membutuhkan otentikasi seperti synaptic, software center atau package manager sedang aktif pada Ubuntu Linux Anda, biasanya kondisi terjadi karena aplikasi-aplikasi yang tersebut sedang aktif, jika ternyata aplikasi-aplikasi tersebut tidak aktif, anda bisa melakukan perintah dibawah ini melalui terminal.

Login Sebagai Root :

    sudo su :

    kemudian input password root

Perintah Terminalnya

    rm /var/lib/apt/lists/lock


