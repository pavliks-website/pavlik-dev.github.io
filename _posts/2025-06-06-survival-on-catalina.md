---
layout: blog
type: post
date: 2025-06-06 17:20:00 +0300
title: Surviving on macOS 10.15 Catalina in 2025
---

*TL;DR: You **still can** survive on 10.15, it’s possible, and still comfortable, but it's still better to move to Ventura on OCLP.*

Apple released the last update for macOS Catalina, Security Update 2022-005, back in 2022, after 3 years since the release.{% include source.html link='https://support.apple.com/en-us/106403' %} As for now (June 6, 2025), the only supported macOS versions are Ventura (13), Sonoma (14), and Sequoia (15).

Unfortunately, macOS Catalina is also the last officially supported version on my Mid-2012 MacBook Pro. I mean yeah, you can use OCLP and install Ventura on it, but something like Sonoma or Sequoia won’t run just as smoothly as Catalina does. (which is already pretty laggy in some places)

So in case you’re having the same problem as me, and you don’t want to install Linux or Windows (which is totally fine), here’s your survival pack for Catalina.

## Browsers

Chrome, as well as Chromium, stopped supporting Catalina after version 129.{% include source.html link='https://support.google.com/chrome/thread/289795700/sunsetting-chrome-support-for-macos-10-15' %} Yes, you can still use 128, but it's already almost a year old.

There is Chromium Legacy, which is a fork of Chromium that supports all macOS versions all the way back to 10.7. Although it crashed on my older MacBook with 10.7.

But, the last release is from May 29, 2024{% include source.html link='https://github.com/blueboxd/chromium-legacy/releases/tag/1303823' %}. Which is already a year old. Plus it's rather laggy. Overall, if you don’t really need a Chromium browser (which is true in most cases), you might try out something else.

Looking at something up-to-date, you might want to try out Firefox. Yeah, not the best option considering last events in Mozilla, but it works. And still supports 10.15.

You can also try LibreWolf, which is a fork of Firefox. It’s Firefox but with a different branding. And some privacy-focused extensions out-of-the-box, which is cool, but that fuckass JS blocker is shit.

If you’re feeling geeky, there’s Pale Moon, a fork of Firefox back in its Classic UI days. Oh and don’t forget Basilisk, same shit but with Australis UI. But it lags for some reason.

Note that these browsers don’t support most of the modern web. Sorry about that. But if your 

## Programming

For something basic like simple HTML pages and Python scripts, Sublime Text 4 will fit perfectly.

But if you want Visual Studio Code, well… It hasn't supported Catalina since March 2025. The February 2025 version works just fine, but you better disable auto updates, because otherwise it’ll break itself trying to auto-update to the latest version (and you guessed it, that doesn’t support Catalina).

If you want Python 3.13 (or even 3.14), it still supports macOS 10.13{% include source.html link='https://www.python.org/downloads/release/python-3140b2/' %}, so you definitely can.

node.js? Hell yeah, I have v22.16.0 installed and it works just as it should.

PHP? Built-in until Monterey.{% include source.html link='https://www.php.net/manual/en/install.macosx.php' %} [Use this tutorial to use it with macOS’s built-in Apache web server.](https://www.php.net/manual/en/install.macosx.bundled.php)

fish shell? 10.9+.{% include source.html link='https://fishshell.com/' %} Go ahead and install it. You might also want to change your default shell with `chsh` or in System Preferences.

Everything else like `git` or `clang` also works.

## Games

I don’t play games much, especially alone, but Roblox{% include source.html link='https://en.help.roblox.com/hc/en-us/articles/203312800-Computer-Hardware-Operating-System-Requirements#h_01HMFCHKY82TP2VQ63X93VRAQK' %} and Minecraft{% include source.html link='https://help.minecraft.net/hc/en-us/articles/4420326353933-Minecraft-Java-Edition-Versions-and-MacOS-' %} work just fine.

Steam stopped supporting Catalina in February 2025, so sorry.{% include source.html link='https://help.steampowered.com/en/faqs/view/736A-892E-4F03-CA38' %}

But Epic Games **does support Catalina!**{% include source.html link='https://www.epicgames.com/help/en-US/c-Category_EpicGamesStore/c-EpicGamesStore_LauncherSupport/system-requirements-for-the-epic-games-launcher-a000084650' %}

## Music

Apple Music still works.

VLC requires at least 10.7.5.

Anything else? An old version will probably work fine.

---

Sooo, I think you still can use Catalina in 2025.

Do you know software that supports Catalina? Let me know and I’ll include it here.

But for now, good luck!
