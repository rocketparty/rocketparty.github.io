---
layout: post
title:  "Laravel on Digital Oceab"
date:   2015-07-23 09:00:00
categories: laravel hosting
tags: laravel php
image: /assets/article_images/2014-08-29-welcome-to-jekyll/desktop.jpg
---


Set up a Digital Ocean Droplet for Laravel/nginx deployment the other day. I used one of the [Digital Ocean guides](https://www.digitalocean.com/community/tutorials/how-to-install-laravel-with-nginx-on-an-ubuntu-12-04-lts-vps) to set the box up. The only real issue I ran into was my Ubuntu version. I'm running 14ish and the guide was written for 12.04. The difference is that mcrypt needs to be explicitly enabled in the latest versions of Ubuntu. The following commands will take care of that.

```
>> php5enmod mcrypt
>> service nginx restart
```
