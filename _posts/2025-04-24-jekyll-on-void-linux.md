---
layout: blog
title: How to install Jekyll on Void Linux
type: post
date: 2025-04-24 10:56:00 +0300
---

Here's how you can install Jekyll on Void Linux:

## 1. Install needed packages

```sh
sudo xbps-install ruby ruby-devel base-devel zlib-devel
```

## 2. Set GEM_HOME variable and add gems/bin to PATH

```sh
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
```

## 3. Restart your terminal and install Jekyll

```sh
gem install jekyll bundler
```

And this is it! Now you have Jekyll installed.

## Note

Please, before installing any gems, run this command:

```sh
bundle config set --local path 'vendor/bundle'
```

This prevents permission hell.
