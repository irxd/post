---
title: 'Test Deep Link Android'
date: '2020-09-11T13:39:31.000Z'
hero_image: ../images/rami-al-zayat-w33-zg-dNL4-unsplash.jpg
---

With ADB:

`$ adb shell am start -a android.intent.action.VIEW -d "deeplink"`

example:
`$ adb shell am start -a android.intent.action.VIEW -d "irxd://myapps"`
___
With Apps:

There are several apps on playstore you can use, search with keyword: test deep link

Reference:
[https://stackoverflow.com/questions/28802115/i-am-trying-to-test-android-deep-link-urls-through-adb-to-launch-my-app](https://stackoverflow.com/questions/28802115/i-am-trying-to-test-android-deep-link-urls-through-adb-to-launch-my-app)