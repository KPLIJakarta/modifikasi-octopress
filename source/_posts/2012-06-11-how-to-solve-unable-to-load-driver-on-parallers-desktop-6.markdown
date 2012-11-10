---
comments: true
date: 2012-06-11 21:54:34
layout: post
slug: how-to-solve-unable-to-load-driver-on-parallers-desktop-6
title: How To Solve Unable To Load Driver On Parallers Desktop 6
wordpress_id: 58
categories:
- Macinthos
---

I'm face this problem when i wanna install new ubuntu version - 12.04 LTS on my mac machine, i just wanna try the new look of it, so i'm decide to using parallers desktop 6 to install ubuntu as virtual machine, but sadly after installation is finish, there are error warning show that parallers unable to load driver.

The answer is just simply add this shell script to terminal. The Problem is this shell script must be run each time your machine boot, my home work is how to execute this shell script automaticly everytime my machine do fresh boot.

    
    sudo kextutil "/Library/Parallels/Parallels Service.app/Contents/Kexts/10.6/prl_hypervisor.kext"
    sudo kextutil "/Library/Parallels/Parallels Service.app/Contents/Kexts/10.6/prl_hid_hook.kext"
    sudo kextutil "/Library/Parallels/Parallels Service.app/Contents/Kexts/10.6/prl_usb_connect.kext"
    sudo kextutil "/Library/Parallels/Parallels Service.app/Contents/Kexts/10.6/prl_netbridge.kext"
    sudo kextutil "/Library/Parallels/Parallels Service.app/Contents/Kexts/10.6/prl_vnic.kext"
    
    <a href="http://passionfactory.files.wordpress.com/2012/06/by-default-2012-06-11-at-10-10-13-pm.png"><img src="http://passionfactory.files.wordpress.com/2012/06/by-default-2012-06-11-at-10-10-13-pm.png" title="by default 2012-06-11 at 10.10.13 PM" height="324" width="519" alt="" class="aligncenter size-full wp-image-62"></img></a>
