---
title: HDR Revolutionizes Gaming with New Update on Dolphin Emulator for Wii/GameCube Classics
date: 2024-09-16T04:11:36.487Z
updated: 2024-09-19T17:36:59.226Z
tags:
  - games
  - tv
  - movies
categories:
  - tech
thumbnail: https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/08/dolphin-emulator-logo-2.jpg
---

## HDR Revolutionizes Gaming with New Update on Dolphin Emulator for Wii/GameCube Classics

It's hard to get emulators _completely_ right with intrincate hardware designs and protections. The first version of Dolphin was released in 2003, but even after 21 years of development, there are still improvements to be made. Dolphin has now published a new progress report outlining all the new features and changes from the past few months, and there's a lot to talk about.

[Dolphin](https://dolphin-emu.org/) has just released its latest progress report, which highlights all the changes that have happened throughout February, March, and April. As a reminder, all of these updates have already been rolled out to Dolphin users, so if you haven't updated your emulator for the past few months, you'll find a lot of improvements here. Many of the changes are under-the-hood adjustments that most people might not notice, and some are even only relevant for developers. Still, they should result in a more stable and faster emulation experience for everyone.

 One of the highlights of this report is a critical security fix addressing a memory safety bug that could have been potentially exploited. A malicious actor could craft a specially crafted game save or exploit a game's functionality to trick Dolphin into performing unsafe memory operations. This could allow them to inject their own code or manipulate existing memory to gain unauthorized control. It doesn't look like this issue was being exploited in the wild, but it's good to see it patched nonetheless.

 There are also a few visual improvements. Errant black pixels around windowed displays have been banished, and an issue causing blurring in some games at 1x native resolution is resolved, resulting in a sharper and cleaner image. Dolphin also introduces full support for custom aspect ratios, complete with aspect ratio corrections—fantastic news if you happen to have an ultra-wide monitor and you wanted to take full advantage of it.

![Dropdown menu with various aspect ratios in Dolphin settings.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/04/aspectratiocustom.png) 

Dolphin

 The emulator can now output to HDR displays on Windows, macOS, and select Linux systems as well. You're getting two HDR enhancement shaders here: AutoHDR subtly expands highlights for an HDR effect while maintaining an authentic look, and PerceptualHDR delivers a more dramatic transformation with higher brightness and saturation. It's worth noting that due to variations in displays and limitations of older game lighting engines, achieving the ideal HDR look may require experimentation and adjustments.

 Another notable improvement here is the addition of Modem Adapter emulation. For the first time ever, the game _Phantasy Star Online Episode I & II Trial Edition_ can be played in Dolphin without modifications. This was previously impossible due to the title's unique requirement for the GameCube Modem Adapter. If you want to play those games online, you can also do that, as custom servers are also supported. You can [see some HDR Dolphin screenshots](https://dolphin-emu.org/blog/2024/04/30/dolphin-progress-report-addendum-hdr-block/) on the project's website, if your device and browser support HDR images.

 Developers also have some good news for themselves as well. For starters, the software JIT profiler was restored. While this feature may not see widespread use, its return is a welcome addition to Dolphin's suite of developer tools, offering even more granular control for those who delve into the emulator's inner workings. You also have the Branch Watch Tool, a robust debugging feature replacing the older Code Diff Tool. Branch Watch gives developers extra tools with advanced code searching and analysis capabilities.

 Finally, with [iOS emulators](https://video-screen-grab.techidaily.com/new-2024-approved-enhancing-mac-use-top-5-recommended-sniping-apps/) being the elephant in the room right now in the emulator world, Dolphin has also provided an update on whether it'll make a version of its emulator for iPhones. Sadly, it looks like it won't be landing on Apple devices, at least for the time being. Due to Apple's strict ban on Just-in-Time (JIT) recompilers in third-party apps, Dolphin cannot be released on iOS or iPadOS. JITs are essential for Dolphin's performance; the emulator's alternative methods like the Interpreter or Cached Interpreter are simply too slow to provide an enjoyable gameplay experience.

 You can [download Dolphin](https://dolphin-emu.org/download/) from the official website for Windows (x86\_64 or 64-bit ARM), macOS (Intel or Apple Silicon), or Android devices. The Android version is also on the [Google Play Store](https://www.anrdoezrs.net/links/3607085/type/dlg/sid/UUhtgUeUpU2002926/https://play.google.com/store/apps/details?id=org.dolphinemu.dolphinemu). Sorry, iPhone owners, you'll have to wait for Apple to relax its restrictions on emulation.

 Source: [Dolphin](https://dolphin-emu.org/blog/2024/04/30/dolphin-progress-report-february-march-and-april-2024/)

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



<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2135353/19272" target="_top" id="2135353">
  <img src="//a.impactradius-go.com/display-ad/19272-2135353" border="0" alt="https://techidaily.com" width="180" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135353/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

