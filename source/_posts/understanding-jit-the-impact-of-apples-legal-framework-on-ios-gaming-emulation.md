---
title: "Understanding JIT: The Impact of Apples Legal Framework on iOS Gaming Emulation"
date: 2024-10-21T20:25:54.732Z
updated: 2024-10-24T11:58:31.541Z
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
<a href="https://dhgate.sjv.io/c/5597632/2106658/12108" target="_top" id="2106658">
  <img src="//a.impactradius-go.com/display-ad/12108-2106658" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://dhgate.sjv.io/i/5597632/2106658/12108" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  What Is JIT?

 JIT compilation is short for "Just In Time" compilation. Compilation is the process of turning programming code into machine code. You can write something in, for example, C code and then compile it for any system, whether it's an x86 CPU as found on most Windows computers or an ARM CPU as found on mobile phones and tablets.

 JIT compilation, as opposed to ahead-of-time compilation, has numerous advantages, not least of which is adaptability to what's currently happening on the computer and what the user is asking the program to do.

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2087234/19272" target="_top" id="2087234">
  <img src="//a.impactradius-go.com/display-ad/19272-2087234" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2087234/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Why Do Emulators Need JIT?

 The developers of emulators have found that the JIT approach lets them achieve levels of performance and efficiency that would otherwise be impossible. Using the JIT technique, the emulated CPU code from the original system can be recompiled to native code for the target host system on the fly. Once that code has been recompiled, it can be cached and used the next time the same call is made without compiling again.

![An iPad running G-Police next a  physical original copy of the game and a PS4 controller](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/an-ipad-running-g-police-next-a-physical-original-copy-of-the-game-and-a-ps4-controller.jpeg) 

Sydney Louw Butler / How-To Geek

 Using the JIT method, it's possible to create self-modifying code, which has become a common approach in video game emulation. This is necessary in some systems because many older systems, particularly cartridge based systems, would load code from the cartridge dynamically and seemingly arbitrarily based on the exact game state. JIT allows for essentially real-time handling of this approach. JIT also lets the emulator optimize the recompiled code to take advantage of the host system as much as possible.

 I'm not a programmer, but even from my point of view, JIT seems like an extremely powerful tool when applied to the tough problem of emulation, based on what I've read.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2129741/7443" target="_top" id="2129741">
  <img src="//a.impactradius-go.com/display-ad/7443-2129741" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2129741/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Why Doesn't Apple Allow JIT?

 Unfortunately, another type of software that can make great use of JIT and self-modifying code is malware. If an app can generate and execute code during its runtime, that opens up the door to all sorts of shenanigans So compiling all the code ahead of time makes it much easier to ensure that the code is safe. Apple also likely doesn't want to have a situation where an app changes its behavior after being approved. Something which can't happen if the pre-compiled code is static.

 The knock-on effect is that software which relies on a JIT recompiler to work at usable speeds won't be approved for the App Store. This is the reason given for the [absence of the popular Dolphin emulator](https://oatmealdome.me/blog/why-dolphin-isnt-coming-to-the-app-store/).

 Of course, there is an alternative to a JIT recompiler, called an "interpreter", but this is many times slower than the JIT method. So while it would work, it would be unplayable. Either we'll have to wait until the iPhone 30 to get the interpreter running fast enough, or we have to hope that Apple loosens its restrictions a little.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2144282/7443" target="_top" id="2144282">
  <img src="//a.impactradius-go.com/display-ad/7443-2144282" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2144282/7443" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://video-capture.techidaily.com/updated-in-2024-master-the-art-of-easy-webinar-recordings-windows-and-macos-advice/"><u>[Updated] In 2024, Master the Art of Easy Webinar Recordings Windows & macOS Advice</u></a></li>
<li><a href="https://buynow-help.techidaily.com/affordable-tech-clean-essentials-the-must-have-kit-for-all-your-devices/"><u>Affordable Tech-Clean Essentials: The Must-Have Kit for All Your Devices</u></a></li>
<li><a href="https://buynow-help.techidaily.com/banana-craze-boosts-value-to-100plus-per-item-in-digital-trading-spotlight-on-steam/"><u>Banana Craze Boosts Value to $100+ per Item in Digital Trading Spotlight on Steam</u></a></li>
<li><a href="https://buynow-help.techidaily.com/beginners-guide-to-staying-active-how-nintendo-systems-make-exercise-fun-and-accessible/"><u>Beginner's Guide to Staying Active: How Nintendo Systems Make Exercise Fun and Accessible</u></a></li>
<li><a href="https://buynow-help.techidaily.com/budget-friendly-twitch-streaming-starts-here-utilizing-equipment-you-likely-own/"><u>Budget-Friendly Twitch Streaming Starts Here: Utilizing Equipment You Likely Own</u></a></li>
<li><a href="https://buynow-help.techidaily.com/bundle-up-your-streaming-unveiling-the-new-dual-subscription-hulu-and-disneyplus-app/"><u>Bundle Up Your Streaming: Unveiling the New Dual-Subscription Hulu & Disney+ App!</u></a></li>
<li><a href="https://buynow-help.techidaily.com/comprehensive-bose-ultra-series-earphones-analysis-the-perfect-companion-for-constant-use/"><u>Comprehensive Bose Ultra Series Earphones Analysis: The Perfect Companion for Constant Use</u></a></li>
<li><a href="https://data-wizards.techidaily.com/easy-tips-to-prevent-video-corruption/"><u>Easy Tips to Prevent Video Corruption</u></a></li>
<li><a href="https://extra-information.techidaily.com/in-2024-best-available-avi-player-cross-platform-compatibility/"><u>In 2024, Best Available AVi Player - Cross-Platform Compatibility</u></a></li>
<li><a href="https://win11.techidaily.com/navigating-the-terrain-of-excessive-disk-space-in-windows/"><u>Navigating the Terrain of Excessive Disk Space in Windows</u></a></li>
<li><a href="https://ai-video-apps.techidaily.com/new-2024-approved-get-splice-video-editing-software-for-mac/"><u>New 2024 Approved Get Splice Video Editing Software for Mac</u></a></li>
<li><a href="https://tech-renaissance.techidaily.com/smartwatch-showdown-googles-new-contender-against-apple-watch-s8-making-the-right-pick-for-your-wrist/"><u>Smartwatch Showdown: Google's New Contender Against Apple Watch S8 | Making the Right Pick for Your Wrist</u></a></li>
<li><a href="https://win-howtos.techidaily.com/troubleshooting-guide-resolving-physxloaderdll-missing-on-launch-issues/"><u>Troubleshooting Guide: Resolving 'PhysXloader.dll' Missing on Launch Issues</u></a></li>
</ul></div>

