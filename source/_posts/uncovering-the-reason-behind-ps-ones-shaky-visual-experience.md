---
title: Uncovering the Reason Behind PS One's Shaky Visual Experience
date: 2024-11-17T16:15:36.794Z
updated: 2024-11-24T17:04:58.431Z
tags:
  - games
  - tv
  - movies
categories:
  - tech
thumbnail: https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/06/a-playstation-1-controller-with-metal-gear-solid-running-on-a-tv-and-a-glitch-effect.jpg
---

## Uncovering the Reason Behind PS One's Shaky Visual Experience

### Highlights

* PlayStation 1 lacked FLOPs due to not having an FPU.
* No Z-buffer resulted in small errors & visible polygons.
* Affine texture mapping caused warping; PS1 trade-offs were speed and cost over complexity.

 Call me biased, but the original PlayStation is still my favorite console of all time. While the games might look a little rough now, they're still as good to play as ever. That said, even back then, PS1 graphics had this signature wobble you didn't find in the competition, so what gives?

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/Vfq0vw0Spz8?si=2EAk6hW-Gb-o33_L&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  It’s All About Floating Points

 Modern GPU performance is often measured ([controversially](https://hardware-help.techidaily.com/brother-hl-2280dw-driver-package-universal-download-for-windows-11-windows-10-windows-8-and-7-users/)) in FLOPs or FLoating Point Operations. This is simply math involving floating point numbers, which in turn are simply whole numbers with a decimal point. The PlayStation's graphics processor had zero FLOPs, because it lacked an FPU or Floating Point Unit. Instead, it uses fixed-point integers to calculate the positions of vertices.

 A "vertice" is a point where two or more lines meet. So in a polygon, which is typically (but not always) a triangle in 3D graphics, there are three vertices. A 3D model consists of multiple polygons, and as that object moves on screen, the positions of the vertices must be calculated in 3D space.

 Since you can only use integers, any position for a vertice that's not an integer will simply be skipped over. So you'll see polygons "snap" between positions with certain types of motion. For example, a character that's standing still and has a subtle idle animation will look like they're jittering a little.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/iOVkXoUxLf4?si=QfC18T2cb5OkiaXo&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Z-Buffer Not Found

 Apart from the lack of an FPU, the PlayStation also lacked a hardware Z-buffer. You might remember XYZ coordinates from school, where you can describe any point within a 3D space using three numbers. The PlayStation lacked a hardware buffer to store depth or Z-axis values, sorted in order of how far away something is from the "camera."

 This meant that game developers had to create their own in-house Z-buffering solution, and since it was not done in hardware, they had to be economical with their depth-sorting algorithms. This led to a common situation in PS1 games where small sorting errors were made and polygons that should have been hidden from view pop in and out of sight.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/vFQCEZiYA08?si=xjIu5IAy77RlHWii&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Affine Texture Mapping Is Not So Fine After All

 Texture mapping is the process of adding textures (which are basically digital pictures) to a polygon wireframe. It's basically the "skin" of a 3D object. The PS1 uses a method known as "affine" texture mapping, which uses simple math to determine the coordinates on the polygon where the texture should be drawn. Affine texture mapping does not take Z-coordinates into account, and so perspective projection will appear incorrect for 3D objects. Remember the PS1 has no Z-buffer!

 Consoles like the Nintendo 64 do have a Z-buffer, and also use a method known as mipmapping, where multiple versions of a texture are swapped out depending on your distance from the object, further improving the clarity and stability of textures in motion. On the PS1, lacking these technologies, it leads to what's known as affine texture warping.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/0Kr7Dpw0HuM?si=05wWDXdPgmC-oBBE&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Fast, Cheap, or Complex: Pick Two

 Different developers did find ways to work around these limitations, and so some PS1 games exhibit these issues to varying degrees. However, trying to address these issues in software almost always means eating up processing power that could have gone to something else. Despite these cutbacks, the PS1's hardware was above all fast. It could pump out polygons faster than anything else at the time.

 It also helps that CRT displays mask most of these issues quite well, and that would have been what the console was designed for. Modern flat panel displays have a negative effect on how PS1 games are presented, making the graphics uglier now than they were back then!

 The bottom line is that the console could have had that extra hardware, but it would have driven the cost up significantly, without any clear benefit to Sony or its players at the time. The company went with "fast and cheap," leaving complexity at the door. History has shown this was the right decision.

##  Emulators Can Correct This (But Should You?)

![An iPad running G-Police next a  physical original copy of the game and a PS4 controller](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/an-ipad-running-g-police-next-a-physical-original-copy-of-the-game-and-a-ps4-controller.jpeg) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/yDuvbv0QOYI?si=byottcEM_Rrvi4EL&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

Sydney Louw Butler / How-To Geek

 If you play PS1 games using one of [many possible emulators](https://some-techniques.techidaily.com/new-immersion-in-hue-and-light-dreamcolors-z32-x-explored/) today, you usually have the option to "fix" most of these problems. We can magically inject floating point values into the game, and clean up texture mapping so the games shine. However, should you do that? There's an argument to be made that these characteristics are part and parcel of the PS1 experience, and just as people don't want to smooth the pixels in their 8- or 16-bit games, I rarely want to remove the wobble from my favorite PS1 titles.

---

 For an excellent explanation from a real game developer and emulation programmer, I highly recommend Modern Vintage Gamer's deep dive into [PS1 graphical warping](https://youtu.be/x8TO-nrUtSI?si=6SUk7e0hBQSiOnoj).

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
<li><a href="https://twitter-videos.techidaily.com/new-2024-approved-mastering-tweet-reactions-a-complete-guide-for-23/"><u>[New] 2024 Approved Mastering Tweet Reactions - A Complete Guide for '23</u></a></li>
<li><a href="https://youtube-docs.techidaily.com/kyrocket-your-channel-to-over-a-million-subscribers/"><u>[New] Skyrocket Your Channel to Over a Million Subscribers</u></a></li>
<li><a href="https://some-tips.techidaily.com/new-tailoring-photos-with-photoshops-dynamic-motion-blur-feature/"><u>[New] Tailoring Photos with Photoshop's Dynamic Motion Blur Feature</u></a></li>
<li><a href="https://some-approaches.techidaily.com/new-unveiling-the-secrets-to-using-vivavideo-app/"><u>[New] Unveiling the Secrets to Using VivaVideo App</u></a></li>
<li><a href="https://screen-recording.techidaily.com/updated-effortless-methods-to-archive-slideshows-for-2024/"><u>[Updated] Effortless Methods to Archive Slideshows for 2024</u></a></li>
<li><a href="https://fox-direct.techidaily.com/updated-exploring-the-best-action-cams-gopros-max-and-hero-11-face-off/"><u>[Updated] Exploring the Best Action Cams GoPro's Max and Hero 11 Face-Off</u></a></li>
<li><a href="https://buynow-help.techidaily.com/discover-elite-audio-upgrades-the-creme-de-la-creme-sound-cards-of-the-2024-market/"><u>Discover Elite Audio Upgrades: The Crème De La Crème Sound Cards of the 2024 Market</u></a></li>
<li><a href="https://buynow-help.techidaily.com/discover-your-inner-adventurer-the-incredible-compact-camera-sx70/"><u>Discover Your Inner Adventurer: The Incredible Compact Camera SX70</u></a></li>
<li><a href="https://buynow-help.techidaily.com/echo-pop-or-echo-dot-understanding-the-key-differences/"><u>Echo Pop or Echo Dot – Understanding The Key Differences</u></a></li>
<li><a href="https://buynow-help.techidaily.com/elysian-estates-transforming-simple-nests-into-grand-homes/"><u>Elysian Estates: Transforming Simple Nests Into Grand Homes</u></a></li>
<li><a href="https://buynow-help.techidaily.com/expert-insights-into-the-samsung-galaxy-watch-active-your-ally-for-personal-fitness-goals/"><u>Expert Insights Into the Samsung Galaxy Watch Active: Your Ally for Personal Fitness Goals</u></a></li>
<li><a href="https://buynow-help.techidaily.com/expert-review-the-strongly-built-uniden-r3-with-exceptional-long-range-features/"><u>Expert Review: The Strongly Built Uniden R3 with Exceptional Long Range Features</u></a></li>
<li><a href="https://buynow-help.techidaily.com/exploring-the-elegance-and-efficiency-of-aukeys-no-nonsense-usb-30-hub-package/"><u>Exploring the Elegance & Efficiency of Aukey's No-Nonsense USB 3.0 Hub Package</u></a></li>
<li><a href="https://buynow-help.techidaily.com/exploring-the-features-of-escort-max-360-high-tech-radar-detection-meets-accurate-gps-navigation/"><u>Exploring the Features of Escort Max 360: High-Tech Radar Detection Meets Accurate GPS Navigation</u></a></li>
<li><a href="https://buynow-help.techidaily.com/fast-and-reliable-or-just-ugly-evaluating-tp-links-av2000-powerline-adapter/"><u>Fast and Reliable or Just Ugly? - Evaluating TP-Link's AV2000 Powerline Adapter</u></a></li>
<li><a href="https://facebook-clips.techidaily.com/fb-videos-to-mp3s-free-online-convert-2023-for-2024/"><u>FB Videos to MP3s - Free Online Convert 2023 for 2024</u></a></li>
<li><a href="https://easy-unlock-android.techidaily.com/in-2024-a-complete-guide-to-oem-unlocking-on-poco-c50-by-drfone-android/"><u>In 2024, A Complete Guide To OEM Unlocking on Poco C50</u></a></li>
<li><a href="https://apple-account.techidaily.com/in-2024-top-notch-solutions-for-disabled-apple-id-on-apple-iphone-11-making-it-possible-by-drfone-ios/"><u>In 2024, Top-Notch Solutions for Disabled Apple ID On Apple iPhone 11 Making It Possible</u></a></li>
<li><a href="https://discover-alternatives.techidaily.com/mastering-tak-audio-formats-unlock-high-quality-music-experience/"><u>Mastering TAK Audio Formats: Unlock High-Quality Music Experience</u></a></li>
</ul></div>

