---
comments: true
date: 2012-06-10 06:26:28
layout: post
slug: creating-your-android-development-environment
title: Creating Your Android Development Environment.
wordpress_id: 20
categories:
- Android
---

This is step by step to creating android development environment, on macinthos, i've been searching that there were less of article on web that discuss about how to prepare your "machine" for android development on macinthos, so here the article.

I'm gonna develop with eclipse, so first thing that i do is downloading and installing eclipse [here](http://www.eclipse.org/downloads/), eclipse web will choose your eclipse version automatic  based on your operating system, i'm choose eclipse classic with 64 bit version.

[![](http://passionfactory.files.wordpress.com/2012/06/by-default-2012-06-10-at-5-46-37-am.png)](http://passionfactory.files.wordpress.com/2012/06/by-default-2012-06-10-at-5-46-37-am.png)

After download finished, extract file in your application directory, just click eclipse icon to run your eclipse. Next step is installing android development tool (ADT Plugin for eclipse). Open eclipse - help - install new software, add https://dl-ssl.google.com/android/eclipse/ url as a repository then click add.

[![](http://passionfactory.files.wordpress.com/2012/06/by-default-2012-06-10-at-6-00-49-am.png)](http://passionfactory.files.wordpress.com/2012/06/by-default-2012-06-10-at-6-00-49-am.png)

in the add repository dialog that appear enter ADT Plugin for name, then click ok, select the checkbox click next and read and accept lisence agreements and restart eclipse after installation completes. Eclipse will ask you what if you wanna install your own android sdk or download the latest SDK, i'm prefer to download the latest sdk that google provide. To install any android component, on eclipse choose window - Android SDK Manager. You can see all status of your android component and sdk package, what if there are any update for your sdk, eclipse will inform you and offer you to install the sdk update.

[![](http://passionfactory.files.wordpress.com/2012/06/by-default-2012-06-10-at-6-11-35-am1.png)](http://passionfactory.files.wordpress.com/2012/06/by-default-2012-06-10-at-6-11-35-am1.png)

Now is installing android virtual device (avd), choice window - avd manager - then click new.

[![](http://passionfactory.files.wordpress.com/2012/06/by-default-2012-06-10-at-6-18-30-am.png)](http://passionfactory.files.wordpress.com/2012/06/by-default-2012-06-10-at-6-18-30-am.png)

If you want to build android application for any platform, you must install al android version on drop down target, for memory i'm choice 256 mb memory to make avd run smoothly, for name section, just write it with your own, then click create avd. Then choose the avd version that you wanna use, then click start and launch. [![](http://passionfactory.files.wordpress.com/2012/06/by-default-2012-06-10-at-6-22-10-am.png)](http://passionfactory.files.wordpress.com/2012/06/by-default-2012-06-10-at-6-22-10-am.png)

And here the final result.

[![](http://passionfactory.files.wordpress.com/2012/06/by-default-2012-06-10-at-6-24-01-am.png)](http://passionfactory.files.wordpress.com/2012/06/by-default-2012-06-10-at-6-24-01-am.png)
