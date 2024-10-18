---
title: Uncovering the Reason Behind PS One's Shaky Visual Experience
date: 2024-10-13T18:07:31.797Z
updated: 2024-10-18T18:36:09.192Z
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

##  It’s All About Floating Points

 Modern GPU performance is often measured ([controversially](https://hardware-help.techidaily.com/brother-hl-2280dw-driver-package-universal-download-for-windows-11-windows-10-windows-8-and-7-users/)) in FLOPs or FLoating Point Operations. This is simply math involving floating point numbers, which in turn are simply whole numbers with a decimal point. The PlayStation's graphics processor had zero FLOPs, because it lacked an FPU or Floating Point Unit. Instead, it uses fixed-point integers to calculate the positions of vertices.

 A "vertice" is a point where two or more lines meet. So in a polygon, which is typically (but not always) a triangle in 3D graphics, there are three vertices. A 3D model consists of multiple polygons, and as that object moves on screen, the positions of the vertices must be calculated in 3D space.

 Since you can only use integers, any position for a vertice that's not an integer will simply be skipped over. So you'll see polygons "snap" between positions with certain types of motion. For example, a character that's standing still and has a subtle idle animation will look like they're jittering a little.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2123731/7443" target="_top" id="2123731">
  <img src="//a.impactradius-go.com/display-ad/7443-2123731" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2123731/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Z-Buffer Not Found

 Apart from the lack of an FPU, the PlayStation also lacked a hardware Z-buffer. You might remember XYZ coordinates from school, where you can describe any point within a 3D space using three numbers. The PlayStation lacked a hardware buffer to store depth or Z-axis values, sorted in order of how far away something is from the "camera."

 This meant that game developers had to create their own in-house Z-buffering solution, and since it was not done in hardware, they had to be economical with their depth-sorting algorithms. This led to a common situation in PS1 games where small sorting errors were made and polygons that should have been hidden from view pop in and out of sight.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2144271/7443" target="_top" id="2144271">
  <img src="//a.impactradius-go.com/display-ad/7443-2144271" border="0" alt="https://techidaily.com" width="600" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2144271/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Affine Texture Mapping Is Not So Fine After All

 Texture mapping is the process of adding textures (which are basically digital pictures) to a polygon wireframe. It's basically the "skin" of a 3D object. The PS1 uses a method known as "affine" texture mapping, which uses simple math to determine the coordinates on the polygon where the texture should be drawn. Affine texture mapping does not take Z-coordinates into account, and so perspective projection will appear incorrect for 3D objects. Remember the PS1 has no Z-buffer!

 Consoles like the Nintendo 64 do have a Z-buffer, and also use a method known as mipmapping, where multiple versions of a texture are swapped out depending on your distance from the object, further improving the clarity and stability of textures in motion. On the PS1, lacking these technologies, it leads to what's known as affine texture warping.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2137412/7443" target="_top" id="2137412">
  <img src="//a.impactradius-go.com/display-ad/7443-2137412" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2137412/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Fast, Cheap, or Complex: Pick Two

 Different developers did find ways to work around these limitations, and so some PS1 games exhibit these issues to varying degrees. However, trying to address these issues in software almost always means eating up processing power that could have gone to something else. Despite these cutbacks, the PS1's hardware was above all fast. It could pump out polygons faster than anything else at the time.

 It also helps that CRT displays mask most of these issues quite well, and that would have been what the console was designed for. Modern flat panel displays have a negative effect on how PS1 games are presented, making the graphics uglier now than they were back then!

 The bottom line is that the console could have had that extra hardware, but it would have driven the cost up significantly, without any clear benefit to Sony or its players at the time. The company went with "fast and cheap," leaving complexity at the door. History has shown this was the right decision.

##  Emulators Can Correct This (But Should You?)

![An iPad running G-Police next a  physical original copy of the game and a PS4 controller](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/an-ipad-running-g-police-next-a-physical-original-copy-of-the-game-and-a-ps4-controller.jpeg) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2043594/7443" target="_top" id="2043594">
  <img src="//a.impactradius-go.com/display-ad/7443-2043594" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2043594/7443" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://digital-screen-recording.techidaily.com/new-2024-approved-the-modern-filmmakers-guide-for-computer-mac-and-mobile/"><u>[New] 2024 Approved The Modern Filmmaker's Guide for Computer, Mac & Mobile</u></a></li>
<li><a href="https://fox-helps.techidaily.com/new-echoes-of-the-past-understanding-sound-overlaps-for-2024/"><u>[New] Echoes of the Past Understanding Sound Overlaps for 2024</u></a></li>
<li><a href="https://fox-hovers.techidaily.com/updated-win-11-mastery-exclusive-less-known-hacks-revealed-for-2024/"><u>[Updated] Win 11 Mastery Exclusive, Less-Known Hacks Revealed for 2024</u></a></li>
<li><a href="https://extra-information.techidaily.com/5-ultimate-platforms-for-high-quality-text-embellishments-for-2024/"><u>5 Ultimate Platforms for High-Quality Text Embellishments for 2024</u></a></li>
<li><a href="https://tech-haven.techidaily.com/art-safety-tactics-thwarting-copycat-ai-algorithms-from-duplicating-originals/"><u>Art Safety Tactics: Thwarting Copycat AI Algorithms From Duplicating Originals</u></a></li>
<li><a href="https://technical-tips.techidaily.com/discover-ios-18-latest-version-released-at-no-cost-with-key-updates-and-insights/"><u>Discover iOS 18 – Latest Version Released at No Cost with Key Updates & Insights</u></a></li>
<li><a href="https://buynow-help.techidaily.com/expert-review-on-the-robust-structure-and-simple-installation-process-for-acurites-pro-station-01036m/"><u>Expert Review on the Robust Structure & Simple Installation Process for AcuRite's Pro Station 01036M</u></a></li>
<li><a href="https://buynow-help.techidaily.com/get-fast-wifi-on-a-budget-comprehensive-review-of-the-tp-link-archer-c80/"><u>Get Fast WiFi on a Budget: Comprehensive Review of the TP-Link Archer C80</u></a></li>
<li><a href="https://easy-unlock-android.techidaily.com/in-2024-how-to-remove-a-previously-synced-google-account-from-your-realme-c33-2023-by-drfone-android/"><u>In 2024, How to Remove a Previously Synced Google Account from Your Realme C33 2023</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/in-2024-how-to-screen-mirroring-oppo-find-x7-drfone-by-drfone-android/"><u>In 2024, How to Screen Mirroring Oppo Find X7? | Dr.fone</u></a></li>
<li><a href="https://buynow-help.techidaily.com/in-depth-analysis-of-cat-s42-tough-mobile-device-robust-defenses-but-modest-performance/"><u>In-Depth Analysis of CAT S42 Tough Mobile Device: Robust Defenses but Modest Performance</u></a></li>
<li><a href="https://buynow-help.techidaily.com/in-depth-evaluation-of-the-oneplus-9-pros-design-velocity-and-imaging-capabilities/"><u>In-Depth Evaluation of the OnePlus 9 Pro's Design, Velocity & Imaging Capabilities</u></a></li>
<li><a href="https://buynow-help.techidaily.com/in-depth-evaluation-pixel-4a-5g-the-perfect-blend-of-affordability-and-cutting-edge-mobile-tech/"><u>In-Depth Evaluation: Pixel 4a 5G - The Perfect Blend of Affordability & Cutting-Edge Mobile Tech</u></a></li>
<li><a href="https://buynow-help.techidaily.com/inside-the-rexing-v1-dashcam-a-perfect-blend-of-discretion-and-dependability/"><u>Inside the Rexing V1 Dashcam: A Perfect Blend of Discretion and Dependability</u></a></li>
<li><a href="https://buynow-help.techidaily.com/is-it-time-to-switch-to-a-state-of-the-art-apple-watch-version/"><u>Is It Time to Switch to a State-of-the-Art Apple Watch Version</u></a></li>
<li><a href="https://buynow-help.techidaily.com/leading-landscape-tripod-the-ultimate-travel-tool/"><u>Leading Landscape Tripod: The Ultimate Travel Tool</u></a></li>
<li><a href="https://win-answers.techidaily.com/resolving-alan-wake-2s-crash-issues-advanced-troubleshooting-guide/"><u>Resolving Alan Wake 2'S Crash Issues - Advanced Troubleshooting Guide</u></a></li>
</ul></div>

