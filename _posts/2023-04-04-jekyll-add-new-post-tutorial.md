---
layout: post
title: Jekyll新增文章教學
date: '2023-04-04 02:15:23 +0800'
---
1. 安裝[Jekyll::Compose](https://github.com/jekyll/jekyll-compose)
此套件可以更簡單的創建文章，無需下載東西。
Add this line to your application's Gemfile:
```
gem 'jekyll-compose', group: [:jekyll_plugins]
```
And then execute:
```shell
bundle
```
2. 新增文章
直接執行以下指令，就會在_posts資料夾裡建立好符合格式的檔案。
```shell
bundle exec jekyll post "My New Post" --timestamp-format "%Y-%m-%d %H:%M:%S %z"
```