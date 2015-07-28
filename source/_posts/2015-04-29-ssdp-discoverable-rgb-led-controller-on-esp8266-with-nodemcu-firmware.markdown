---
layout: post
title: "SSDP discoverable RGB LED controller on ESP8266 with NodeMCU firmware"
date: 2015-04-29 17:49:58 +0300
comments: true
categories: [ESP8266, NodeMCU, IoT]
author: Artem Pastukhov
---
## NodeMCU rgb led controller with SSDP capability.

# Installation

* You should use latest firmware from [nodemcu-firmware](https://github.com/nodemcu/nodemcu-firmware) with multicast support
* Grab the sources from [nodemcu-ssdp](https://github.com/pastukhov/nodemcu-ssdp)
* Place these files on top of [NodeMCU-httpserver](https://github.com/marcoskirsch/nodemcu-httpserver).
* Add upnp.lua and http/rgb.lua to list of files to compile.
* Add dofile("upnp.lc") after dofile("httpserver.lc")(80).
* Yo should see "OVOI RGB controller" in your upnp browser.
* It is working  at least in windows network browser and upnp-inspector.
