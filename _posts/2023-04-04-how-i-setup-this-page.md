---
layout: post
title: 如何建置此網站（Jekyll + Cirpy theme + Github page）
date: '2023-04-04 02:30:26 +0800'
---
## Step 1: 跟著[Jekyll](https://jekyllrb.com/docs/)官方文件把環境裝一裝
我是使用Mac，可以看到第一步驟有個[prerequisites](https://jekyllrb.com/docs/installation/)，雖然mac內建ruby，但官方推薦安裝他們指定的版本。
    
1. 先安裝[Homebrew](https://brew.sh) 
    可以看這個[影片](https://youtu.be/HUzxCZD4IhI)教學
2. 用homebrew安裝`chruby`和`ruby-install`
    ```shell
    brew install chruby ruby-install xz
    ```
3. 安裝指定的ruby版本
    ```shell
    ruby-install ruby 3.1.3
    ```
4. 當執行ruby時，自動變成跑chruby
    ```shell
    echo "source $(brew --prefix)/opt/chruby/share/chruby/chruby.sh" >> ~/.zshrc
    echo "source $(brew --prefix)/opt/chruby/share/chruby/auto.sh" >> ~/.zshrc
    echo "chruby ruby-3.1.3" >> ~/.zshrc # run 'chruby' to see actual version
    ```
5. 確認ruby版本
    有更動zshrc，所以要重開一個terminal（cmd+T）
    ```shell
    ruby -v
    ```
    It should show ruby 3.1.3p185 (2022-11-24 revision 1a6b16756e) or a newer version.
6.  用gems安裝Jekyll和bundler
    ```shell
    gem install jekyll bundler
    ```

## Step 2: 跟著[Chirpy Doc](https://chirpy.cotes.page/posts/getting-started/)繼續安裝
1. Sign in to GitHub and browse to [Chirpy Starter](https://github.com/cotes2020/chirpy-starter), click the button `Use this template` > `Create a new repository`, and name the new repository `USERNAME.github.io`, where `USERNAME` represents your GitHub username.
2. 把他clone到本地
3. Installing Dependencies
    ```shell
    bundle
    ```
4. 在本地測試
    ```shell
    bundle exec jekyll s
    ```
5. Configuration修改
    到`_config.yml`修改相關的東西。
