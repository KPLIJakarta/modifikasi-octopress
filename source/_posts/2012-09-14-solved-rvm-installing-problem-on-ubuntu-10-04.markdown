---
comments: true
date: 2012-09-14 07:51:07
layout: post
slug: solved-rvm-installing-problem-on-ubuntu-10-04
title: '[SOLVED] RVM Installing Problem On Ubuntu 10.04'
wordpress_id: 282
categories:
- Ruby
---

Jadi .bashrc pelakunya.

File .baschrc is a hidden file, you need ls -a to show it up

    root@syaifulbahri-laptop:/home/syaifulbahri# ls -a

Then you need to edit your .bashrc file

    vim .bashrc

Replace Baris Ini

    [ -z "$PS1" ] && return

Dengan ini

    if [[ -n "$PS1" ]]; then

Kemudian tambahkan pada line terakhir .bashrc

    if [[ -s $HOME/.rvm/scripts/rvm ]] ; then source $HOME/.rvm/scripts/rvm ; fi

    fi

Sesuaikan dengan direktori user anda

Terakhir reload file .bashrc

    source ~/.bashrc

Ujicoba RVM kembali dengan

    rvm notes

There You Go...
