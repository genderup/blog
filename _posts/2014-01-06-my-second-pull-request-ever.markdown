---
layout: post
title:  "My second pull request ever"
date:   2014-01-01 13:18:08
categories: open source
---

Things went so well the first time--my first pull request ever was merged into NodeBB--that I decided to jump right back in with some more code, but this time to a differnet project. Do you know <a href="http://chat.meatspac.es">chat meatspace</a>? Very fun! It's inspired several projects, one being <a href="http://meatbunch.es">meatbunch.es</a> which listens for posts from chat meatspace via sockets and arranges gits into a Brady Bunch style logo

<img src="https://dl.dropboxusercontent.com/u/10328969/meatbunches.png" width=500 height=500>

Currently, if the same person posts eight chats in a row to chat meatspace, meatbunch will fill all eight squares with the same person. Since that's not how the Brady Bunch actually works, I added some code to make sure each box showed a different person. This was pretty easy to do since Meatspace saves a fingerprint for each user.   I only had to grab the fingerprint for each message, save it to a fingerprints array, and check whether it was already present in the array. If it was, I just returned. Meatbunch also lets you click on a gif to remove it from the squares. In that case, the fingerprint would have to be removed from the array so the person could be allowed back in if they post again to chat meatspace. 

<a href="https://github.com/llkats/meatbunches/pull/5">Link to pull request</a>