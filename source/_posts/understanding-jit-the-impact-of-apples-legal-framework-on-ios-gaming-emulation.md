---
title: "Understanding JIT: The Impact of Apples Legal Framework on iOS Gaming Emulation"
date: 2024-10-07T18:58:00.178Z
updated: 2024-10-12T17:08:37.306Z
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
<a href="https://aligracehair.sjv.io/c/5597632/1902304/19272" target="_top" id="1902304">
  <img src="//a.impactradius-go.com/display-ad/19272-1902304" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1902304/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  What Is JIT?

 JIT compilation is short for "Just In Time" compilation. Compilation is the process of turning programming code into machine code. You can write something in, for example, C code and then compile it for any system, whether it's an x86 CPU as found on most Windows computers or an ARM CPU as found on mobile phones and tablets.

 JIT compilation, as opposed to ahead-of-time compilation, has numerous advantages, not least of which is adaptability to what's currently happening on the computer and what the user is asking the program to do.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2100538/7443" target="_top" id="2100538">
  <img src="//a.impactradius-go.com/display-ad/7443-2100538" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2100538/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Why Do Emulators Need JIT?

 The developers of emulators have found that the JIT approach lets them achieve levels of performance and efficiency that would otherwise be impossible. Using the JIT technique, the emulated CPU code from the original system can be recompiled to native code for the target host system on the fly. Once that code has been recompiled, it can be cached and used the next time the same call is made without compiling again.

![An iPad running G-Police next a  physical original copy of the game and a PS4 controller](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/an-ipad-running-g-police-next-a-physical-original-copy-of-the-game-and-a-ps4-controller.jpeg) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2144271/7443" target="_top" id="2144271">
  <img src="//a.impactradius-go.com/display-ad/7443-2144271" border="0" alt="https://techidaily.com" width="600" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2144271/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

Sydney Louw Butler / How-To Geek

 Using the JIT method, it's possible to create self-modifying code, which has become a common approach in video game emulation. This is necessary in some systems because many older systems, particularly cartridge based systems, would load code from the cartridge dynamically and seemingly arbitrarily based on the exact game state. JIT allows for essentially real-time handling of this approach. JIT also lets the emulator optimize the recompiled code to take advantage of the host system as much as possible.

 I'm not a programmer, but even from my point of view, JIT seems like an extremely powerful tool when applied to the tough problem of emulation, based on what I've read.

##  Why Doesn't Apple Allow JIT?

 Unfortunately, another type of software that can make great use of JIT and self-modifying code is malware. If an app can generate and execute code during its runtime, that opens up the door to all sorts of shenanigans So compiling all the code ahead of time makes it much easier to ensure that the code is safe. Apple also likely doesn't want to have a situation where an app changes its behavior after being approved. Something which can't happen if the pre-compiled code is static.

 The knock-on effect is that software which relies on a JIT recompiler to work at usable speeds won't be approved for the App Store. This is the reason given for the [absence of the popular Dolphin emulator](https://oatmealdome.me/blog/why-dolphin-isnt-coming-to-the-app-store/).

 Of course, there is an alternative to a JIT recompiler, called an "interpreter", but this is many times slower than the JIT method. So while it would work, it would be unplayable. Either we'll have to wait until the iPhone 30 to get the interpreter running fast enough, or we have to hope that Apple loosens its restrictions a little.

<!-- affiliate ads begin -->
<a href="https://laganoo.pxf.io/c/5597632/1528703/16446" target="_top" id="1528703">
  <img src="//a.impactradius-go.com/display-ad/16446-1528703" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://laganoo.pxf.io/i/5597632/1528703/16446" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://fox-helps.techidaily.com/new-crafting-visual-tales-the-essential-guide-to-text-effects-for-2024/"><u>[New] Crafting Visual Tales The Essential Guide to Text Effects for 2024</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/new-filmmaking-faceoff-hero-session-x-or-polaroid-cube/"><u>[New] Filmmaking Faceoff Hero Session X or Polaroid Cube?</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/new-in-2024-quick-fix-to-spot-instagram-disconnects/"><u>[New] In 2024, Quick Fix to Spot Instagram Disconnects</u></a></li>
<li><a href="https://fox-access.techidaily.com/new-key-destinations-enhancing-youtube-video-impact-for-2024/"><u>[New] Key Destinations Enhancing YouTube Video Impact for 2024</u></a></li>
<li><a href="https://blog-min.techidaily.com/ai-powers-live-translations-in-microsoft-edge-redefining-multimedia-accessibility/"><u>AI Powers Live Translations in Microsoft Edge, Redefining Multimedia Accessibility</u></a></li>
<li><a href="https://buynow-help.techidaily.com/comprehensive-guide-vyncs-link-tracking-features-and-perplexing-subscription-options/"><u>Comprehensive Guide: Vyncs Link Tracking Features and Perplexing Subscription Options</u></a></li>
<li><a href="https://buynow-help.techidaily.com/expertly-curated-selection-of-brands-and-phones-at-reputable-retailers/"><u>Expertly Curated Selection of Brands and Phones at Reputable Retailers</u></a></li>
<li><a href="https://android-transfer.techidaily.com/how-to-transfer-data-from-lava-blaze-curve-5g-to-other-android-devices-drfone-by-drfone-transfer-from-android-transfer-from-android/"><u>How to Transfer Data from Lava Blaze Curve 5G to Other Android Devices? | Dr.fone</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/in-2024-why-does-the-pokemon-go-battle-league-not-available-on-nokia-c110-drfone-by-drfone-virtual-android/"><u>In 2024, Why does the pokemon go battle league not available On Nokia C110 | Dr.fone</u></a></li>
<li><a href="https://buynow-help.techidaily.com/inside-the-lenovo-ideapad-130s-laptop-compact-efficiency-meets-exceptional-functionality/"><u>Inside the Lenovo IdeaPad 130S Laptop: Compact Efficiency Meets Exceptional Functionality</u></a></li>
<li><a href="https://tech-recovery.techidaily.com/m4a-to-mpeg-konvertisseur-online-bonusgratis-betreffend-movavi/"><u>M4A-to-MPEG Konvertisseur Online Bonusgratis - Betreffend Movavi</u></a></li>
<li><a href="https://buynow-help.techidaily.com/maximizing-your-network-a-thorough-review-of-netgear-nighthawk-x6-wireless-expansion-technology/"><u>Maximizing Your Network: A Thorough Review of Netgear Nighthawk X6 Wireless Expansion Technology</u></a></li>
<li><a href="https://buynow-reviews.techidaily.com/protecting-previewed-photos-within-your-microsoft-word-documents/"><u>Protecting Previewed Photos Within Your Microsoft Word Documents</u></a></li>
<li><a href="https://buynow-help.techidaily.com/review-of-lgs-latest-smartphone-a-blend-of-elegant-design-and-reliable-stylus-feature/"><u>Review of LG's Latest Smartphone: A Blend of Elegant Design & Reliable Stylus Feature</u></a></li>
<li><a href="https://buynow-help.techidaily.com/unveiling-the-performance-of-linksyss-wrt1900acs-an-in-depth-look-at-an-open-source-wi-fi-gateway/"><u>Unveiling the Performance of Linksys's WRT1900ACS: An In-Depth Look at an Open-Source Wi-Fi Gateway</u></a></li>
<li><a href="https://buynow-help.techidaily.com/unveiling-the-powerhouse-detailed-examination-of-the-huion-kamvas-gt-191-pen-display-for-professional-artists/"><u>Unveiling the Powerhouse: Detailed Examination of the Huion Kamvas GT-191 Pen Display for Professional Artists</u></a></li>
<li><a href="https://buynow-help.techidaily.com/yakuza-like-a-dragon-revealed-the-unmissable-turnkey-to-the-world-of-engaging-rpg-gaming/"><u>Yakuza: Like a Dragon Revealed – The Unmissable Turnkey to the World of Engaging RPG Gaming</u></a></li>
</ul></div>

