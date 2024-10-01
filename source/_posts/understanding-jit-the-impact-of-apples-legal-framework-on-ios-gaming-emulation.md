---
title: "Understanding JIT: The Impact of Apples Legal Framework on iOS Gaming Emulation"
date: 2024-09-27T16:04:48.502Z
updated: 2024-10-01T17:58:38.021Z
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
<a href="https://aligracehair.sjv.io/c/5597632/1918679/19272" target="_top" id="1918679">
  <img src="//a.impactradius-go.com/display-ad/19272-1918679" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1918679/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  What Is JIT?

 JIT compilation is short for "Just In Time" compilation. Compilation is the process of turning programming code into machine code. You can write something in, for example, C code and then compile it for any system, whether it's an x86 CPU as found on most Windows computers or an ARM CPU as found on mobile phones and tablets.

 JIT compilation, as opposed to ahead-of-time compilation, has numerous advantages, not least of which is adaptability to what's currently happening on the computer and what the user is asking the program to do.

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1972693/19272" target="_top" id="1972693">
  <img src="//a.impactradius-go.com/display-ad/19272-1972693" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1972693/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Why Do Emulators Need JIT?

 The developers of emulators have found that the JIT approach lets them achieve levels of performance and efficiency that would otherwise be impossible. Using the JIT technique, the emulated CPU code from the original system can be recompiled to native code for the target host system on the fly. Once that code has been recompiled, it can be cached and used the next time the same call is made without compiling again.

![An iPad running G-Police next a  physical original copy of the game and a PS4 controller](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/an-ipad-running-g-police-next-a-physical-original-copy-of-the-game-and-a-ps4-controller.jpeg) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1918661/19272" target="_top" id="1918661">
  <img src="//a.impactradius-go.com/display-ad/19272-1918661" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1918661/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

Sydney Louw Butler / How-To Geek

 Using the JIT method, it's possible to create self-modifying code, which has become a common approach in video game emulation. This is necessary in some systems because many older systems, particularly cartridge based systems, would load code from the cartridge dynamically and seemingly arbitrarily based on the exact game state. JIT allows for essentially real-time handling of this approach. JIT also lets the emulator optimize the recompiled code to take advantage of the host system as much as possible.

 I'm not a programmer, but even from my point of view, JIT seems like an extremely powerful tool when applied to the tough problem of emulation, based on what I've read.

<!-- affiliate ads begin -->
<a href="https://review-au.sjv.io/c/5597632/2135316/14409" target="_top" id="2135316">
  <img src="//a.impactradius-go.com/display-ad/14409-2135316" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://review-au.sjv.io/i/5597632/2135316/14409" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Why Doesn't Apple Allow JIT?

 Unfortunately, another type of software that can make great use of JIT and self-modifying code is malware. If an app can generate and execute code during its runtime, that opens up the door to all sorts of shenanigans So compiling all the code ahead of time makes it much easier to ensure that the code is safe. Apple also likely doesn't want to have a situation where an app changes its behavior after being approved. Something which can't happen if the pre-compiled code is static.

 The knock-on effect is that software which relies on a JIT recompiler to work at usable speeds won't be approved for the App Store. This is the reason given for the [absence of the popular Dolphin emulator](https://oatmealdome.me/blog/why-dolphin-isnt-coming-to-the-app-store/).

 Of course, there is an alternative to a JIT recompiler, called an "interpreter", but this is many times slower than the JIT method. So while it would work, it would be unplayable. Either we'll have to wait until the iPhone 30 to get the interpreter running fast enough, or we have to hope that Apple loosens its restrictions a little.

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
<li><a href="https://facebook.techidaily.com/1719153181758-satoshi-sheep-the-ceos-animal-mashup-moniker/"><u>'Satoshi Sheep': The CEO's Animal Mashup Moniker</u></a></li>
<li><a href="https://facebook-video-recording.techidaily.com/new-how-to-make-your-facebook-video-stand-out/"><u>[New] How to Make Your Facebook Video Stand Out</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/new-in-2024-quickly-add-speech-overlays-to-your-instagram-posts/"><u>[New] In 2024, Quickly Add Speech Overlays to Your Instagram Posts</u></a></li>
<li><a href="https://fox-hovers.techidaily.com/new-mastering-easy-underwater-film-making-top-7-hacks/"><u>[New] Mastering Easy Underwater Film-Making Top 7 Hacks</u></a></li>
<li><a href="https://article-knowledge.techidaily.com/updated-2024-approved-premium-screens-at-their-peak-top-10-listings-for-4k-monitors/"><u>[Updated] 2024 Approved Premium Screens at Their Peak Top #10 Listings for 4K Monitors</u></a></li>
<li><a href="https://buynow-help.techidaily.com/comprehensive-evaluation-of-tp-link-re200-ac750-wifi-signal-booster-a-cost-effective-choice/"><u>Comprehensive Evaluation of TP-Link RE200 AC750 WiFi Signal Booster - A Cost-Effective Choice</u></a></li>
<li><a href="https://buynow-help.techidaily.com/comprehensive-guide-to-the-space-empires-in-stellaris/"><u>Comprehensive Guide to the Space Empires in Stellaris</u></a></li>
<li><a href="https://buynow-help.techidaily.com/comprehensive-review-of-the-top-race-rc-rock-crawler-for-unbeatable-off-road-performance/"><u>Comprehensive Review of the Top Race RC Rock Crawler for Unbeatable Off-Road Performance</u></a></li>
<li><a href="https://buynow-help.techidaily.com/discovering-b550-xt-revolutionary-voice-management/"><u>Discovering B550-XT: Revolutionary Voice Management</u></a></li>
<li><a href="https://buynow-help.techidaily.com/discovering-the-mini-marvel-a-comprehensive-samsung-galaxy-s10e-evaluation/"><u>Discovering the Mini Marvel: A Comprehensive Samsung Galaxy S10e Evaluation</u></a></li>
<li><a href="https://buynow-help.techidaily.com/effortless-accuracy-and-enduring-connections-the-sabrent-mini-travel-wireless-mouse-experience/"><u>Effortless Accuracy & Enduring Connections: The Sabrent Mini Travel Wireless Mouse Experience</u></a></li>
<li><a href="https://data-safeguard.techidaily.com/elevate-online-presence-using-cookiebots-tools/"><u>Elevate Online Presence Using Cookiebot's Tools</u></a></li>
<li><a href="https://buynow-help.techidaily.com/ergodriven-topo-mat-assessment-a-must-have-anti-fatigue-standing-pad-for-office-productivity/"><u>Ergodriven Topo Mat Assessment: A Must-Have Anti-Fatigue Standing Pad for Office Productivity</u></a></li>
<li><a href="https://buynow-help.techidaily.com/experience-comfort-with-the-ergodriven-topo-the-anti-fatigue-mat-for-effortless-long-stands-at-your-desk/"><u>Experience Comfort with the Ergodriven Topo - The Anti-Fatigue Mat for Effortless Long Stands at Your Desk</u></a></li>
<li><a href="https://some-techniques.techidaily.com/full-exploration-of-picsarts-new-features-for-2024/"><u>Full Exploration of PicsArt's New Features for 2024</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/in-2024-how-can-i-get-more-stardust-in-pokemon-go-on-lava-yuva-2-pro-drfone-by-drfone-virtual-android/"><u>In 2024, How can I get more stardust in pokemon go On Lava Yuva 2 Pro? | Dr.fone</u></a></li>
<li><a href="https://win11-tips.techidaily.com/mastering-the-art-of-reopening-calendars-and-mail/"><u>Mastering the Art of Reopening Calendars and Mail</u></a></li>
</ul></div>

