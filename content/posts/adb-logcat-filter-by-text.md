---
title: 'ADB Logcat Filter by Text'
date: '2022-03-27T11:09:31.000Z'
hero_image: ../images/04-sai-kiran-anagani-Tjbk79TARiE-unsplash.jpg
---

With single text:

`$ adb logcat | grep 'keyword'`

example:
`$ adb logcat | grep 'sentry'`
___
With multi text:

`$ adb logcat | grep -E 'keyword|keyword-n'`

example:
`$ adb logcat | grep -E 'sentry|alert'`