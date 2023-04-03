---
layout: post
title: Jekyll新增文章教學
date: '2023-04-04 02:15:23 +0800'
categories: [其他]
tags: [jekyll]
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
> 文章其他設定，例如：新增tag與category，請參見[文件](https://chirpy.cotes.page/posts/write-a-new-post/)。
3. 本地測試
```shell
bundle exec jekyll s
```
4. 更新到github上
```shell
bundle
git add .
git commit -m "add post"
git push
```