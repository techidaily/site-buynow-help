---
title: "Understanding JIT: The Impact of Apples Legal Framework on iOS Gaming Emulation"
date: 2024-11-10T20:47:38.347Z
updated: 2024-11-15T07:51:07.328Z
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
<a href="https://aligracehair.sjv.io/c/5597632/1934288/19272" target="_top" id="1934288">
  <img src="//a.impactradius-go.com/display-ad/19272-1934288" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1934288/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  What Is JIT?

 JIT compilation is short for "Just In Time" compilation. Compilation is the process of turning programming code into machine code. You can write something in, for example, C code and then compile it for any system, whether it's an x86 CPU as found on most Windows computers or an ARM CPU as found on mobile phones and tablets.

 JIT compilation, as opposed to ahead-of-time compilation, has numerous advantages, not least of which is adaptability to what's currently happening on the computer and what the user is asking the program to do.

##  Why Do Emulators Need JIT?

 The developers of emulators have found that the JIT approach lets them achieve levels of performance and efficiency that would otherwise be impossible. Using the JIT technique, the emulated CPU code from the original system can be recompiled to native code for the target host system on the fly. Once that code has been recompiled, it can be cached and used the next time the same call is made without compiling again.

![An iPad running G-Police next a  physical original copy of the game and a PS4 controller](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/an-ipad-running-g-police-next-a-physical-original-copy-of-the-game-and-a-ps4-controller.jpeg) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1896555/19272" target="_top" id="1896555">
  <img src="//a.impactradius-go.com/display-ad/19272-1896555" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1896555/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

Sydney Louw Butler / How-To Geek

 Using the JIT method, it's possible to create self-modifying code, which has become a common approach in video game emulation. This is necessary in some systems because many older systems, particularly cartridge based systems, would load code from the cartridge dynamically and seemingly arbitrarily based on the exact game state. JIT allows for essentially real-time handling of this approach. JIT also lets the emulator optimize the recompiled code to take advantage of the host system as much as possible.

 I'm not a programmer, but even from my point of view, JIT seems like an extremely powerful tool when applied to the tough problem of emulation, based on what I've read.

<!-- affiliate ads begin -->
<span id="1938141">
					<video width="576" height="240" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1938141.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/22993-1938141">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1938141.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:360px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fhomestyler.sjv.io%2Fc%2F5597632%2F1938141%2F22993'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1938141/22993" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Why Doesn't Apple Allow JIT?

 Unfortunately, another type of software that can make great use of JIT and self-modifying code is malware. If an app can generate and execute code during its runtime, that opens up the door to all sorts of shenanigans So compiling all the code ahead of time makes it much easier to ensure that the code is safe. Apple also likely doesn't want to have a situation where an app changes its behavior after being approved. Something which can't happen if the pre-compiled code is static.

 The knock-on effect is that software which relies on a JIT recompiler to work at usable speeds won't be approved for the App Store. This is the reason given for the [absence of the popular Dolphin emulator](https://oatmealdome.me/blog/why-dolphin-isnt-coming-to-the-app-store/).

 Of course, there is an alternative to a JIT recompiler, called an "interpreter", but this is many times slower than the JIT method. So while it would work, it would be unplayable. Either we'll have to wait until the iPhone 30 to get the interpreter running fast enough, or we have to hope that Apple loosens its restrictions a little.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2087408/7443" target="_top" id="2087408">
  <img src="//a.impactradius-go.com/display-ad/7443-2087408" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2087408/7443" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://extra-guidance.techidaily.com/new-perfecting-every-shots-hue-the-essential-11-tutorials-on-color-adjustment/"><u>[New] Perfecting Every Shot's Hue The Essential 11 Tutorials on Color Adjustment</u></a></li>
<li><a href="https://youtube-web.techidaily.com/ising-stars-in-digital-domain/"><u>[New] Rising Stars in Digital Domain</u></a></li>
<li><a href="https://some-guidance.techidaily.com/new-switching-between-safe-mode-and-picture-in-picture-on-iosmacos/"><u>[New] Switching Between Safe Mode & Picture In Picture on iOS/MacOS</u></a></li>
<li><a href="https://screen-recording.techidaily.com/2024-approved-mov-saving-on-the-go-top-six-tips-to-improve-your-workflow-in-windows-11/"><u>2024 Approved .MOV Saving on the Go - Top Six Tips to Improve Your Workflow in Windows 11</u></a></li>
<li><a href="https://buynow-help.techidaily.com/comprehensive-analysis-of-the-acurite-pro-01036m-effortless-setup-and-solid-structure/"><u>Comprehensive Analysis of the AcuRite Pro 01036M: Effortless Setup and Solid Structure</u></a></li>
<li><a href="https://buynow-help.techidaily.com/comprehensive-escort-max-t-360-analysis-advanced-radar-and-gps-detector-unveiled/"><u>Comprehensive Escort Max T 360 Analysis - Advanced Radar & GPS Detector Unveiled</u></a></li>
<li><a href="https://buynow-help.techidaily.com/comprehensive-review-is-the-mohu-leaf-30-a-worthy-match-in-price-and-performance/"><u>Comprehensive Review: Is the Mohu Leaf 30 a Worthy Match in Price and Performance?</u></a></li>
<li><a href="https://buynow-help.techidaily.com/comprehensive-samsung-galaxy-note20-ultra-5g-smartphone-evaluation/"><u>Comprehensive Samsung Galaxy Note20 Ultra 5G Smartphone Evaluation</u></a></li>
<li><a href="https://buynow-help.techidaily.com/deciding-on-a-nintendo-console-switch-lite-vs-switch-oled-your-complete-guide/"><u>Deciding on a Nintendo Console? Switch Lite Vs. Switch OLED - Your Complete Guide</u></a></li>
<li><a href="https://buynow-help.techidaily.com/discover-restorative-slumber-the-ultimate-ihome-zenergy-bedside-machine-analysis/"><u>Discover Restorative Slumber: The Ultimate IHome Zenergy Bedside Machine Analysis</u></a></li>
<li><a href="https://buynow-help.techidaily.com/discover-the-affordable-side-of-premium-pet-trackers/"><u>Discover the Affordable Side of Premium Pet Trackers</u></a></li>
<li><a href="https://unlock-android.techidaily.com/how-to-enable-usb-debugging-on-a-locked-zte-blade-a73-5g-phone-by-drfone-android/"><u>How To Enable USB Debugging on a Locked ZTE Blade A73 5G Phone</u></a></li>
<li><a href="https://fox-access.techidaily.com/master-quick-red-eye-correction-in-iphone-photos-for-free-for-2024/"><u>Master Quick Red-Eye Correction in iPhone Photos for FREE for 2024</u></a></li>
<li><a href="https://win-manuals.techidaily.com/mastering-scene-creation-with-flipprograms-overcoming-potential-restrictions/"><u>Mastering Scene Creation with FlipPrograms: Overcoming Potential Restrictions</u></a></li>
<li><a href="https://win-extraordinary.techidaily.com/step-by-step-tutorial-modifying-display-settings-in-windows-11s-hyper-v-environment/"><u>Step-by-Step Tutorial: Modifying Display Settings in Windows 11'S Hyper-V Environment</u></a></li>
</ul></div>

