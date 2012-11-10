---
comments: true
date: 2012-11-05 19:36:36
layout: post
slug: so-thats-new-ios-phonegap-works
title: So, That's New iOS Phonegap Works
wordpress_id: 370
categories:
- iOS
---

Just curious, i'm not talk about kind of web development way to build iOS app, because for any reason [i'm move to native development,](http://passionfactory.wordpress.com/2012/07/22/im-going-native/) this evening my friend tell me that my article about[ using phonegap development to build iOS app](http://passionfactory.wordpress.com/2012/06/11/installing-cordova-1-8-on-x-code-4-3-2-for-ios-development/) is not work again on new phonegap version, after browsing on [phonegap site](http://phonegap.com) on developer getting started guide section, yeah there were new kind of method to make iOS based phonegap work, and here's the method



	
  1. As usual, you must download new phonegap version [here](http://phonegap.com)

	
  2. Extract to your own directory

	
  3. Make sure that you have Xcode & Xcode command line tools installed, you can find it on Mac App Store

	
  4. Phonegap for iOS location is on lib/ios

	
  5. Lauch terminal, move your directory to bin folder location on your phonegap extracted app


Lets write thing

    
    ./create <project_folder_path> <package_name> <project_name> then press "Enter"


See my code below for detail

    
    ./create /Users/tragicidea/Desktop/HelloWorld org.apache.HelloWorld HelloWorld


Open the project folder as you describe above

[![](http://passionfactory.files.wordpress.com/2012/11/screen-shot-2012-11-05-at-7-31-43-pm.png)](http://passionfactory.files.wordpress.com/2012/11/screen-shot-2012-11-05-at-7-31-43-pm.png)



Open your Xcode Project File, then run it on simulator

[![](http://passionfactory.files.wordpress.com/2012/11/screen-shot-2012-11-05-at-7-33-33-pm.png)](http://passionfactory.files.wordpress.com/2012/11/screen-shot-2012-11-05-at-7-33-33-pm.png)

When you're ready, you gonna have this

[![](http://passionfactory.files.wordpress.com/2012/11/screen-shot-2012-11-05-at-7-35-00-pm.png)](http://passionfactory.files.wordpress.com/2012/11/screen-shot-2012-11-05-at-7-35-00-pm.png)










