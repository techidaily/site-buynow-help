---
title: "Expanded Compatibility: Raspberry Pi's New Update Enables Connection with 32-Bit Systems"
date: 2024-08-28 23:14:58
updated: 2024-08-29 10:21:38
tags:
  - games
  - tv
  - movies
categories:
  - tech
thumbnail: https://thmb.techidaily.com/1003c2d436af1af88200a4fecafa1c9b55219d7d2c61adc69cde92d0a51179ae.jpg
---

## Expanded Compatibility: Raspberry Pi's New Update Enables Connection with 32-Bit Systems

It's been just over a month since the launch of Raspberry Pi Connect, an official remote access tool that allows you to control your Pi computer from a web browser. Today, Raspberry Pi Connect is rolling out support for 32-bit Pi computers. The new Connect release also includes a remote shell access feature.

[Raspberry Pi Connect](https://snapchat-videos.techidaily.com/new-2024-approved-mastering-mobile-screen-recording-in-snapchat/) was limited to 64-bit Pi computers at launch. In other words, it only worked on the Pi 4, Pi 5, and Pi 400\. Newfound 32-bit support brings Connect to _all_ models of Pi computer, including the original Raspberry Pi from 2012, the tiny Raspberry Pi Zero, and so on.

 There's a big caveat here—remote desktop functionality doesn't work on 32-bit Pi models. If you set up Raspberry Pi Connect with an old 32-bit SBC, you will be limited to remote shell access (which is itself a new feature). This is also true of 64-bit Pi computers that haven't been updated to Pi OS Bookworm, as remote desktop requires a Wayland compositor. A Pi 4 that hasn't been updated to the latest OS version cannot use desktop mirroring.

![Remote shell access through Raspberry Pi Connect.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/06/65.jpg) 

The Raspberry Pi Foundation

 I doubt that these limitations will be a "problem." Remote shell access from a terminal window is more convenient and powerful than desktop mirroring. And because 32-bit Pi models are often relegated to headless applications, the lack of desktop mirroring may go unnoticed by most users. You can't mirror a desktop that doesn't exist.

 The Raspberry Pi team also confirms that advanced Pi Connect functionality, including remote file transfer, are currently in development. I'm surprised that remote file transfer wasn't included at launch, but maybe it doesn't matter, as FireZilla and other FTP applications already fill this role.

 You can set up Pi Connect by following the instructions listed in the [Raspberry Pi Documentation](https://www.raspberrypi.com/documentation/services/connect.html). The setup process is incredibly easy and should only take you a few minutes. Note that remote desktop and shell access functionality are still in beta and suffer from [some known issues](https://www.raspberrypi.com/documentation/services/connect.html#known-issues). Also, users may encounter latency when relaying is required, as Pi Connect currently relies on just one TURN relay server.

 Source: [The Raspberry Pi Foundation](https://www.raspberrypi.com/news/raspberry-pi-connect-remote-shell-access-and-support-for-older-devices/)

<ins class="adsbygoogle"
     style="display:block"
     data-ad-format="autorelaxed"
     data-ad-client="ca-pub-7571918770474297"
     data-ad-slot="1223367746"></ins>



<ins class="adsbygoogle"
     style="display:block"
     data-ad-client="ca-pub-7571918770474297"
     data-ad-slot="8358498916"
     data-ad-format="auto"
     data-full-width-responsive="true"></ins>
