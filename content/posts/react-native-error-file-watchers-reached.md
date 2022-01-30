---
title: 'React Native Error ENOSPC: System limit for number of file watchers reached on Linux'
date: '2020-08-10T00:50:31.000Z'
hero_image: ../images/02-max-chen-lud4OaUCP4Q-unsplash.jpg
---

Problem: Error when installing/running react native package on Linux

Root Cause: The number of files monitored(hot reload) has reached the limit

Solution: 
Increase Inotify(package that Linux use to observe filesystem events) max limit
1. open config file `$ sudo nano /etc/sysctl.conf`
2. add `fs.inotify.max_user_watches=524288` at the bottom file, save and exit
3. load the new config `$ sudo sysctl -p`

Reference:
[https://stackoverflow.com/questions/55763428/react-native-error-enospc-system-limit-for-number-of-file-watchers-reached](https://stackoverflow.com/questions/55763428/react-native-error-enospc-system-limit-for-number-of-file-watchers-reached)