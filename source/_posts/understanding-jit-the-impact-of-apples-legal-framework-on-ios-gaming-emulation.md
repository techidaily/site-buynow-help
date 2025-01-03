---
title: "Understanding JIT: The Impact of Apples Legal Framework on iOS Gaming Emulation"
date: 2025-01-01T16:09:24.073Z
updated: 2025-01-03T16:59:12.264Z
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/fm0XhU5H8R4?si=cFPk6XK3X3CQSI7Y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  What Is JIT?

 JIT compilation is short for "Just In Time" compilation. Compilation is the process of turning programming code into machine code. You can write something in, for example, C code and then compile it for any system, whether it's an x86 CPU as found on most Windows computers or an ARM CPU as found on mobile phones and tablets.

 JIT compilation, as opposed to ahead-of-time compilation, has numerous advantages, not least of which is adaptability to what's currently happening on the computer and what the user is asking the program to do.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/bofw6eJA7Bg?si=HM2gKZGH4L1otw3e" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Why Do Emulators Need JIT?

 The developers of emulators have found that the JIT approach lets them achieve levels of performance and efficiency that would otherwise be impossible. Using the JIT technique, the emulated CPU code from the original system can be recompiled to native code for the target host system on the fly. Once that code has been recompiled, it can be cached and used the next time the same call is made without compiling again.

![An iPad running G-Police next a  physical original copy of the game and a PS4 controller](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/an-ipad-running-g-police-next-a-physical-original-copy-of-the-game-and-a-ps4-controller.jpeg) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/QRaEdFMU-Xc?si=OjaiTvlogJy5wHhN" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

Sydney Louw Butler / How-To Geek

 Using the JIT method, it's possible to create self-modifying code, which has become a common approach in video game emulation. This is necessary in some systems because many older systems, particularly cartridge based systems, would load code from the cartridge dynamically and seemingly arbitrarily based on the exact game state. JIT allows for essentially real-time handling of this approach. JIT also lets the emulator optimize the recompiled code to take advantage of the host system as much as possible.

 I'm not a programmer, but even from my point of view, JIT seems like an extremely powerful tool when applied to the tough problem of emulation, based on what I've read.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/it8VkxDUdAc?si=ef6VZWR7kW4P9ikh" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Why Doesn't Apple Allow JIT?

 Unfortunately, another type of software that can make great use of JIT and self-modifying code is malware. If an app can generate and execute code during its runtime, that opens up the door to all sorts of shenanigans So compiling all the code ahead of time makes it much easier to ensure that the code is safe. Apple also likely doesn't want to have a situation where an app changes its behavior after being approved. Something which can't happen if the pre-compiled code is static.

 The knock-on effect is that software which relies on a JIT recompiler to work at usable speeds won't be approved for the App Store. This is the reason given for the [absence of the popular Dolphin emulator](https://oatmealdome.me/blog/why-dolphin-isnt-coming-to-the-app-store/).

 Of course, there is an alternative to a JIT recompiler, called an "interpreter", but this is many times slower than the JIT method. So while it would work, it would be unplayable. Either we'll have to wait until the iPhone 30 to get the interpreter running fast enough, or we have to hope that Apple loosens its restrictions a little.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/rBnnLFJbvr4?si=LlHYrYlOBp7NLMec" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://facebook-video-footage.techidaily.com/updated-streamlined-method-for-crafting-mobile-focused-youtube-channels/"><u>[Updated] Streamlined Method for Crafting Mobile-Focused YouTube Channels</u></a></li>
<li><a href="https://some-guidance.techidaily.com/updated-top-50plus-overlays-for-engaging-media-content/"><u>[Updated] Top 50+ Overlays for Engaging Media Content</u></a></li>
<li><a href="https://screen-activity-recording.techidaily.com/8-superior-windows-video-call-apps-ranked-for-2024/"><u>8 Superior Windows Video Call Apps Ranked for 2024</u></a></li>
<li><a href="https://driver-error.techidaily.com/bluetooth-driver-update-for-lenovo-on-windows-11/"><u>Bluetooth Driver Update for Lenovo on Windows 11</u></a></li>
<li><a href="https://mondly-stories.techidaily.com/bridge-cultures-master-more-languages/"><u>Bridge Cultures: Master More Languages</u></a></li>
<li><a href="https://techidaily.com/different-methods-for-resetting-vivo-y56-5g-phones-with-screen-locked-and-not-drfone-by-drfone-reset-android-reset-android/"><u>Different Methods for Resetting Vivo Y56 5G Phones with Screen Locked and Not | Dr.fone</u></a></li>
<li><a href="https://buynow-help.techidaily.com/discover-how-bouncies-connected-drive-device-offers-simple-navigation-for-less/"><u>Discover How Bouncie's Connected Drive Device Offers Simple Navigation for Less!</u></a></li>
<li><a href="https://buynow-help.techidaily.com/experience-a-great-convertible-and-inexpensive-asus-chromebook-with-our-detailed-review/"><u>Experience a Great, Convertible & Inexpensive Asus Chromebook with Our Detailed Review</u></a></li>
<li><a href="https://buynow-help.techidaily.com/experience-enhanced-connectivity-with-synology-rt2600ac-wi-fi-router-parental-controls-included/"><u>Experience Enhanced Connectivity with Synology RT2600ac Wi-Fi Router: Parental Controls Included</u></a></li>
<li><a href="https://buynow-help.techidaily.com/exploring-the-beantech-bitwatch-s1-plus-an-in-depth-review-of-a-stellar-budget-smartwatch-choice/"><u>Exploring the Beantech Bitwatch S1 Plus - An In-Depth Review of a Stellar Budget Smartwatch Choice</u></a></li>
<li><a href="https://buynow-help.techidaily.com/inside-the-ps4-pro-review-how-sony-transforms-standard-playstation-4-into-a-4k-powerhouse/"><u>Inside the PS4 Pro Review: How Sony Transforms Standard PlayStation 4 Into a 4K Powerhouse</u></a></li>
<li><a href="https://buynow-help.techidaily.com/samsung-galaxy-tab-s7plus-review-a-premium-android-powerhouse/"><u>Samsung Galaxy Tab S7+ Review: A Premium Android Powerhouse</u></a></li>
<li><a href="https://data-safeguard.techidaily.com/top-10-expertly-curated-software-selections-to-recover-lost-data-on-iphones-ios-17-ready/"><u>Top 10 Expertly Curated Software Selections to Recover Lost Data on iPhones (iOS 17 Ready)</u></a></li>
<li><a href="https://iphone-unlock.techidaily.com/unlocking-iphone-xs-passcode-without-a-computer-drfone-by-drfone-ios/"><u>Unlocking iPhone XS Passcode without a Computer | Dr.fone</u></a></li>
<li><a href="https://buynow-help.techidaily.com/user-guide-test-drive-the-google-nest-doorbell-with-batteries/"><u>User Guide: Test Drive the Google Nest Doorbell with Batteries</u></a></li>
</ul></div>

