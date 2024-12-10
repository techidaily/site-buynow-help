---
title: "Understanding JIT: The Impact of Apples Legal Framework on iOS Gaming Emulation"
date: 2024-12-03T21:43:37.652Z
updated: 2024-12-10T08:56:10.998Z
tags:
  - games
  - tv
  - movies
categories:
  - tech
thumbnail: https://thmb.techidaily.com/5bcf8cebc4ec75a2f2c5443679e92acacca4bb84ee860e6fb058bd25619e5c79.jpg
---

## Understanding JIT: The Impact of Apples Legal Framework on iOS Gaming Emulation

### Key Takeaways

* JIT compilation is crucial for emulator performance, but Apple restricts it for security reasons.
* Emulators use JIT to optimize performance by recompiling code on the fly.
* Apple's limitations may change, but for now, emulator users must wait or consider jailbreaking.

 While Apple seems to have opened the floodgates when it comes to emulator apps on iPhone, iPad, and Apple TV, you may have noticed that certain systems are conspicuously missing from the menu. There's a good chance that's because of a specific feature known as "JIT" compilation being restricted by App Store rules.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/5FWCFI3f_cs?si=Kt2Onr_E4c616tbH" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  What Is JIT?

 JIT compilation is short for "Just In Time" compilation. Compilation is the process of turning programming code into machine code. You can write something in, for example, C code and then compile it for any system, whether it's an x86 CPU as found on most Windows computers or an ARM CPU as found on mobile phones and tablets.

 JIT compilation, as opposed to ahead-of-time compilation, has numerous advantages, not least of which is adaptability to what's currently happening on the computer and what the user is asking the program to do.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/zXUt81WsQpI?si=W3DKIAsa2-qbGadJ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Why Do Emulators Need JIT?

 The developers of emulators have found that the JIT approach lets them achieve levels of performance and efficiency that would otherwise be impossible. Using the JIT technique, the emulated CPU code from the original system can be recompiled to native code for the target host system on the fly. Once that code has been recompiled, it can be cached and used the next time the same call is made without compiling again.

![An iPad running G-Police next a  physical original copy of the game and a PS4 controller](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/an-ipad-running-g-police-next-a-physical-original-copy-of-the-game-and-a-ps4-controller.jpeg) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/eu4vwlZcMvM?si=4vEczfVU4BUUFP-t" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

Sydney Louw Butler / How-To Geek

 Using the JIT method, it's possible to create self-modifying code, which has become a common approach in video game emulation. This is necessary in some systems because many older systems, particularly cartridge based systems, would load code from the cartridge dynamically and seemingly arbitrarily based on the exact game state. JIT allows for essentially real-time handling of this approach. JIT also lets the emulator optimize the recompiled code to take advantage of the host system as much as possible.

 I'm not a programmer, but even from my point of view, JIT seems like an extremely powerful tool when applied to the tough problem of emulation, based on what I've read.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/PKZUYice-ws?si=L8iMa9T3h7TMSWdQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Why Doesn't Apple Allow JIT?

 Unfortunately, another type of software that can make great use of JIT and self-modifying code is malware. If an app can generate and execute code during its runtime, that opens up the door to all sorts of shenanigans So compiling all the code ahead of time makes it much easier to ensure that the code is safe. Apple also likely doesn't want to have a situation where an app changes its behavior after being approved. Something which can't happen if the pre-compiled code is static.

 The knock-on effect is that software which relies on a JIT recompiler to work at usable speeds won't be approved for the App Store. This is the reason given for the [absence of the popular Dolphin emulator](https://oatmealdome.me/blog/why-dolphin-isnt-coming-to-the-app-store/).

 Of course, there is an alternative to a JIT recompiler, called an "interpreter", but this is many times slower than the JIT method. So while it would work, it would be unplayable. Either we'll have to wait until the iPhone 30 to get the interpreter running fast enough, or we have to hope that Apple loosens its restrictions a little.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/6xGqSETroqA?si=4C1GPgXi-AksR_oO" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Things Could Still Change

 It's early days for the emulation scene on the mainstream App Store. Apple may yet decide to loosen this requirement for emulators, or adapt its policies to ensure an adequate level of security for these apps. This will likely be something that's worked out between those approving apps and those developing them. 

 Of course, this issue doesn't exist for those who jailbreak their devices, which lets them [sideload](https://tech-haven.techidaily.com/navigating-nuance-the-human-advantage-over-bots/)any code they like. However, I wouldn't recommend anyone to do that without a terribly good reason, and for most people the downsides of jailbreaking simply aren't worth being able to play retro games on their i-devices.

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

<span class="atpl-alsoreadstyle">Also read:</span>
<div><ul>
<li><a href="https://discord-videos.techidaily.com/updated-discord-for-music-lovers-adding-spotify-support/"><u>[Updated] Discord for Music Lovers Adding Spotify Support</u></a></li>
<li><a href="https://fox-hovers.techidaily.com/a-closer-look-at-sonys-s6700-enhancements-for-2024/"><u>A Closer Look at Sony's S6700 Enhancements for 2024</u></a></li>
<li><a href="https://ios-pokemon-go.techidaily.com/a-detailed-pokemon-go-pvp-tier-list-to-make-you-a-pro-trainer-for-apple-iphone-15-pro-drfone-by-drfone-virtual-ios/"><u>A Detailed Pokemon Go PvP Tier List to Make you a Pro Trainer For Apple iPhone 15 Pro | Dr.fone</u></a></li>
<li><a href="https://fake-location.techidaily.com/complete-tutorial-to-use-vpna-to-fake-gps-location-on-honor-magic5-ultimate-drfone-by-drfone-virtual-android/"><u>Complete Tutorial to Use VPNa to Fake GPS Location On Honor Magic5 Ultimate | Dr.fone</u></a></li>
<li><a href="https://buynow-reviews.techidaily.com/discover-the-topmost-wearable-fitness-gadgets/"><u>Discover the Topmost Wearable Fitness Gadgets</u></a></li>
<li><a href="https://technical-tips.techidaily.com/dive-into-the-world-of-free-tunes-explore-our-selection-of-7-best-streaming-melody-makers-on-android-and-apple-phones/"><u>Dive Into the World of Free Tunes - Explore Our Selection of 7 Best Streaming Melody Makers on Android & Apple Phones</u></a></li>
<li><a href="https://fox-friendly.techidaily.com/how-to-get-100k-view-on-youtube-video-for-2024/"><u>How to Get 100K View on YouTube Video for 2024</u></a></li>
<li><a href="https://android-transfer.techidaily.com/in-2024-two-ways-to-sync-contacts-from-google-pixel-7a-to-gmail-drfone-by-drfone-transfer-from-android-transfer-from-android/"><u>In 2024, Two Ways to Sync Contacts from Google Pixel 7a to Gmail | Dr.fone</u></a></li>
<li><a href="https://buynow-help.techidaily.com/reinventing-mobile-working-space-dive-into-the-features-of-the-msi-pro-mp161-e2-portable-display/"><u>Reinventing Mobile Working Space: Dive Into the Features of the MSI PRO MP161 E2 Portable Display</u></a></li>
<li><a href="https://buynow-help.techidaily.com/reviewing-excellence-in-android-tablets-discover-what-makes-the-samsung-galaxy-tab-s7-shine/"><u>Reviewing Excellence in Android Tablets - Discover What Makes the Samsung Galaxy Tab S7 Shine</u></a></li>
<li><a href="https://buynow-help.techidaily.com/simplifying-connectivity-a-complete-review-of-google-wifi-your-essential-mesh-router-companion/"><u>Simplifying Connectivity: A Complete Review of Google WiFi, Your Essential Mesh Router Companion</u></a></li>
<li><a href="https://buynow-help.techidaily.com/step-by-step-setup-for-the-ultimate-protection-with-blinks-outdoor-cameras/"><u>Step-by-Step Setup for the Ultimate Protection with Blink's Outdoor Cameras</u></a></li>
<li><a href="https://buynow-help.techidaily.com/the-ultimate-guide-to-advanced-tech-tools-for-tranquil-slumber/"><u>The Ultimate Guide to Advanced Tech Tools for Tranquil Slumber</u></a></li>
<li><a href="https://tech-haven.techidaily.com/ultimate-guide-how-to-effortlessly-extract-audio-from-videos-on-pcs-with-windows-10-or-11-including-bulk-processing/"><u>Ultimate Guide: How to Effortlessly Extract Audio From Videos on PCs with Windows 10 or 11, Including Bulk Processing</u></a></li>
</ul></div>

