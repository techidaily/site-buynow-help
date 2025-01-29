---
title: "Understanding JIT: The Impact of Apples Legal Framework on iOS Gaming Emulation"
date: 2025-01-25T23:03:24.262Z
updated: 2025-01-29T18:09:38.513Z
tags:
  - games
  - tv
  - movies
categories:
  - tech
thumbnail: https://thmb.techidaily.com/5bcf8cebc4ec75a2f2c5443679e92acacca4bb84ee860e6fb058bd25619e5c79.jpg
---

## Understanding JIT: The Impact of Apples Legal Framework on iOS Gaming Emulation

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/793ViIxl4tI?si=DDBkjPlPX5bZ-f1Y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

### Key Takeaways

* JIT compilation is crucial for emulator performance, but Apple restricts it for security reasons.
* Emulators use JIT to optimize performance by recompiling code on the fly.
* Apple's limitations may change, but for now, emulator users must wait or consider jailbreaking.

 While Apple seems to have opened the floodgates when it comes to emulator apps on iPhone, iPad, and Apple TV, you may have noticed that certain systems are conspicuously missing from the menu. There's a good chance that's because of a specific feature known as "JIT" compilation being restricted by App Store rules.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/UUPt2zKtJ5k?si=LLHdsFDLzVByJsKj" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  What Is JIT?

 JIT compilation is short for "Just In Time" compilation. Compilation is the process of turning programming code into machine code. You can write something in, for example, C code and then compile it for any system, whether it's an x86 CPU as found on most Windows computers or an ARM CPU as found on mobile phones and tablets.

 JIT compilation, as opposed to ahead-of-time compilation, has numerous advantages, not least of which is adaptability to what's currently happening on the computer and what the user is asking the program to do.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/0Kr7Dpw0HuM?si=05wWDXdPgmC-oBBE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Why Do Emulators Need JIT?

 The developers of emulators have found that the JIT approach lets them achieve levels of performance and efficiency that would otherwise be impossible. Using the JIT technique, the emulated CPU code from the original system can be recompiled to native code for the target host system on the fly. Once that code has been recompiled, it can be cached and used the next time the same call is made without compiling again.

![An iPad running G-Police next a  physical original copy of the game and a PS4 controller](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/an-ipad-running-g-police-next-a-physical-original-copy-of-the-game-and-a-ps4-controller.jpeg) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/jjGL9wFdlbo?si=Vb1JgZqRXNc03UGG" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

Sydney Louw Butler / How-To Geek

 Using the JIT method, it's possible to create self-modifying code, which has become a common approach in video game emulation. This is necessary in some systems because many older systems, particularly cartridge based systems, would load code from the cartridge dynamically and seemingly arbitrarily based on the exact game state. JIT allows for essentially real-time handling of this approach. JIT also lets the emulator optimize the recompiled code to take advantage of the host system as much as possible.

 I'm not a programmer, but even from my point of view, JIT seems like an extremely powerful tool when applied to the tough problem of emulation, based on what I've read.

##  Why Doesn't Apple Allow JIT?

 Unfortunately, another type of software that can make great use of JIT and self-modifying code is malware. If an app can generate and execute code during its runtime, that opens up the door to all sorts of shenanigans So compiling all the code ahead of time makes it much easier to ensure that the code is safe. Apple also likely doesn't want to have a situation where an app changes its behavior after being approved. Something which can't happen if the pre-compiled code is static.

 The knock-on effect is that software which relies on a JIT recompiler to work at usable speeds won't be approved for the App Store. This is the reason given for the [absence of the popular Dolphin emulator](https://oatmealdome.me/blog/why-dolphin-isnt-coming-to-the-app-store/).

 Of course, there is an alternative to a JIT recompiler, called an "interpreter", but this is many times slower than the JIT method. So while it would work, it would be unplayable. Either we'll have to wait until the iPhone 30 to get the interpreter running fast enough, or we have to hope that Apple loosens its restrictions a little.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/FLlUft1ZxI0?si=pBd5QdHEE27qsNlN" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://fox-hovers.techidaily.com/new-in-2024-mobile-cinema-apples-no1-8-pack-free-and-paid-film-app-guide/"><u>[New] In 2024, Mobile Cinema Apple's No.1, 8-Pack Free & Paid Film App Guide</u></a></li>
<li><a href="https://visual-screen-recording.techidaily.com/new-the-ultimate-guide-to-video-call-capturing-on-devices/"><u>[New] The Ultimate Guide to Video Call Capturing on Devices</u></a></li>
<li><a href="https://win-bits.techidaily.com/windows-1187discord/"><u>两种方法：怎样在Windows 11、8或7系统中找回删除的Discord图片</u></a></li>
<li><a href="https://buynow-help.techidaily.com/compact-and-powerful-a-review-of-sx620-hs-by-canon/"><u>Compact & Powerful - A Review of SX620 HS by Canon</u></a></li>
<li><a href="https://fox-triigers.techidaily.com/discover-both-cost-free-and-subscription-based-methods-for-modifying-mts-video-format/"><u>Discover Both Cost-Free and Subscription-Based Methods for Modifying MTS Video Format</u></a></li>
<li><a href="https://buynow-info.techidaily.com/exploring-the-acer-aspire-c27-the-ultimate-compact-and-versatile-desktop-computer/"><u>Exploring the Acer Aspire C27: The Ultimate Compact and Versatile Desktop Computer</u></a></li>
<li><a href="https://buynow-help.techidaily.com/exploring-the-unexpected-depths-of-yokus-island-express-an-enchanting-journey-revealed/"><u>Exploring the Unexpected Depths of Yoku's Island Express – An Enchanting Journey Revealed</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/how-to-stream-anything-from-vivo-v29-pro-to-apple-tv-drfone-by-drfone-android/"><u>How To Stream Anything From Vivo V29 Pro to Apple TV | Dr.fone</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/in-2024-how-to-screen-mirroring-xiaomi-13t-drfone-by-drfone-android/"><u>In 2024, How to Screen Mirroring Xiaomi 13T? | Dr.fone</u></a></li>
<li><a href="https://buynow-help.techidaily.com/navigating-the-world-of-digital-books-an-in-depth-review-of-amazons-kindle-oasis-2019/"><u>Navigating the World of Digital Books: An In-Depth Review of Amazon's Kindle Oasis (2019)</u></a></li>
<li><a href="https://tech-recovery.techidaily.com/secure-and-style-the-best-iphone-se-case-collection-of-2022-to-shield-and-enhance-pcmag/"><u>Secure & Style - The Best iPhone SE Case Collection of 2022 to Shield and Enhance | PCMag</u></a></li>
<li><a href="https://buynow-help.techidaily.com/top-ranked-gaming-mini-pcs-ultimate-buyers-guide/"><u>Top-Ranked Gaming Mini PCs: Ultimate Buyers Guide</u></a></li>
<li><a href="https://screen-video-capture.techidaily.com/unveiling-methods-to-record-and-preserve-internet-broadcasts-for-2024/"><u>Unveiling Methods to Record and Preserve Internet Broadcasts for 2024</u></a></li>
</ul></div>

