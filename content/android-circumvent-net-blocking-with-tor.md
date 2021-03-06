+++
date = "2016-03-21T20:42:52-04:00"
title = "Android: Circumvent Internet restrictions with Tor"
description = "Your work around Internet blocking on an Android device"

+++

> The Tor browser was released since I wrote this article. You can [download it from Google Play](https://play.google.com/store/apps/details?id=org.torproject.torbrowser). Still, everything below is valid and useful for more specific requirements.

This guide will help you work around restricted Internet connection like a school network or Turkish Internet service provider that blocks Twitter.

## Orbot and Orfox

When using the Tor Browser bundle what you get is a modified version of Firefox which bundles the Tor proxy. Firefox then connects through that proxy to the Tor network. On an Android device, the browser and proxy come as two apps.

[Orbot](https://guardianproject.info/apps/orbot/) is the proxy. It's packed with features and is quite flexible.

[Orfox](https://guardianproject.info/apps/orfox/) is the browser. It's a modified version of Firefox with built-in security modules and options you'll need.

You need to do is install both apps.

### Google Play

The simplest method is to install via Google Play.

[Orbot](https://play.google.com/store/apps/details?id=org.torproject.android) [Orfox](https://play.google.com/store/apps/details?id=info.guardianproject.orfox)

### F-Droid

If you cannot or do not want to use Google Play there's hope. F-Droid is an alternative market place for Android [free and open source software](/what-is-free-software/).

* Visit the [F-Droid](https://f-droid.org) website.
* Hit the install button and complete installation.
* Start F-Droid.
* Hit the menu icon on the top right corner.
* Choose "Repositories".
* Enable "Guardian Project Official Releases".
* Disable everything else.
* Exit by hitting the left arrow in front of "Repositories".
* Hit the refresh circle arrow next to the menu icon.
* Wait for the update to finish.
* Search for "Orbot".
* Install "Tor (anonymity) client".
* Search for "Orfox".
* Install "Orfox: Tor Browser for Android".

## Configs

By default, Orbot starts on boot. You might want to disable that since Orfox will start Orbot when it needs.

To access Orbot config panel open the app and hit the sliders icon on the top right corner.

Adding [uBlock Origin](https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/) to Orfox can help with load times. But it helps fingerprint your browser since it has non-standard config. If you care anonymity, don't install.

## Tor is blocked

If for any reason, your connection to the Tor network is blocked, there's a trick you can try.

Open Orbot and hit the bridges button on the bottom right. Choose an obfuscation method and give the app some time to work. There's no visual indicator and the logs are a bit hard to read so make sure you wait at least 30 seconds. Open Orfox and check if you're connected.

If that fails tries another obfuscation method. If they fail, choose "get new bridges" as an obfuscation method and follow instructions. Try all the obfuscation methods again.

## Accessing Twitter

Visit twitter.com with Orfox and click the link at the end of the following sentence => "Or, you can go temporarily to this **mobile site**".

If you want to use Twitter Android app, you need to set those proxy settings => "Proxy Host": localhost, "Proxy Port" 8118. You can access the Proxy options from the login or sign up by opening the app menu on the top right corner. If you are logged in you need to open => menu, settings, location and proxy.

## It doesn't work

If you've followed the steps and aren't connecting to Tor let me know. Contact me. I will help you out.

