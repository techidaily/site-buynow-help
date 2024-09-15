---
title: Uncovering the Reason Behind PS One's Shaky Visual Experience
date: 2024-09-13T09:13:18.216Z
updated: 2024-09-14T21:50:49.120Z
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

##  Z-Buffer Not Found

 Apart from the lack of an FPU, the PlayStation also lacked a hardware Z-buffer. You might remember XYZ coordinates from school, where you can describe any point within a 3D space using three numbers. The PlayStation lacked a hardware buffer to store depth or Z-axis values, sorted in order of how far away something is from the "camera."

 This meant that game developers had to create their own in-house Z-buffering solution, and since it was not done in hardware, they had to be economical with their depth-sorting algorithms. This led to a common situation in PS1 games where small sorting errors were made and polygons that should have been hidden from view pop in and out of sight.

##  Affine Texture Mapping Is Not So Fine After All

 Texture mapping is the process of adding textures (which are basically digital pictures) to a polygon wireframe. It's basically the "skin" of a 3D object. The PS1 uses a method known as "affine" texture mapping, which uses simple math to determine the coordinates on the polygon where the texture should be drawn. Affine texture mapping does not take Z-coordinates into account, and so perspective projection will appear incorrect for 3D objects. Remember the PS1 has no Z-buffer!

 Consoles like the Nintendo 64 do have a Z-buffer, and also use a method known as mipmapping, where multiple versions of a texture are swapped out depending on your distance from the object, further improving the clarity and stability of textures in motion. On the PS1, lacking these technologies, it leads to what's known as affine texture warping.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2118311/7443" target="_top" id="2118311">
  <img src="//a.impactradius-go.com/display-ad/7443-2118311" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2118311/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Fast, Cheap, or Complex: Pick Two

 Different developers did find ways to work around these limitations, and so some PS1 games exhibit these issues to varying degrees. However, trying to address these issues in software almost always means eating up processing power that could have gone to something else. Despite these cutbacks, the PS1's hardware was above all fast. It could pump out polygons faster than anything else at the time.

 It also helps that CRT displays mask most of these issues quite well, and that would have been what the console was designed for. Modern flat panel displays have a negative effect on how PS1 games are presented, making the graphics uglier now than they were back then!

 The bottom line is that the console could have had that extra hardware, but it would have driven the cost up significantly, without any clear benefit to Sony or its players at the time. The company went with "fast and cheap," leaving complexity at the door. History has shown this was the right decision.

<!-- affiliate ads begin -->
<a href="https://unicoeye.pxf.io/c/5597632/2134218/18498" target="_top" id="2134218">
  <img src="//a.impactradius-go.com/display-ad/18498-2134218" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://unicoeye.pxf.io/i/5597632/2134218/18498" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Emulators Can Correct This (But Should You?)

![An iPad running G-Police next a  physical original copy of the game and a PS4 controller](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/an-ipad-running-g-police-next-a-physical-original-copy-of-the-game-and-a-ps4-controller.jpeg) 

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
<li><a href="https://vp-tips.techidaily.com/updated-strategies-for-streaming-fb-live-on-zoom-platform-for-2024/"><u>[Updated] Strategies for Streaming FB Live on Zoom Platform for 2024</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/best-pokemons-for-pvp-matches-in-pokemon-go-for-samsung-galaxy-a23-5g-drfone-by-drfone-virtual-android/"><u>Best Pokemons for PVP Matches in Pokemon Go For Samsung Galaxy A23 5G | Dr.fone</u></a></li>
<li><a href="https://video-screen-grab.techidaily.com/google-translate-strategies-for-excellent-audio-to-text/"><u>Google Translate Strategies for Excellent Audio to Text</u></a></li>
<li><a href="https://activate-lock.techidaily.com/in-2024-the-most-effective-ways-to-bypass-apple-iphone-8-plus-activation-lock-by-drfone-ios/"><u>In 2024, The Most Effective Ways to Bypass Apple iPhone 8 Plus Activation Lock</u></a></li>
<li><a href="https://audio-shaping.techidaily.com/new-how-to-mix-audio-tracks-into-one-file-for-a-video-for-2024/"><u>New How to Mix Audio Tracks Into One File for A Video for 2024</u></a></li>
<li><a href="https://fox-that.techidaily.com/resolved-why-arent-my-iphone-contacts-displaying-troubleshooting-steps-inside/"><u>Resolved! Why Aren't My iPhone Contacts Displaying? Troubleshooting Steps Inside</u></a></li>
<li><a href="https://hardware-updates.techidaily.com/synaptic-touchpad-driver-update-made-easy-for-all-users/"><u>Synaptic Touchpad Driver Update Made Easy for All Users</u></a></li>
<li><a href="https://buynow-help.techidaily.com/the-amazing-featherweight-contender-a-thorough-review-of-the-high-performing-lg-gram-17-laptop/"><u>The Amazing Featherweight Contender – A Thorough Review of the High-Performing LG Gram 17 Laptop</u></a></li>
<li><a href="https://buynow-help.techidaily.com/the-perfect-balance-of-elegance-and-economy-in-depth-look-into-the-acclaimed-fossil-sport-collection/"><u>The Perfect Balance of Elegance & Economy - In-Depth Look Into the Acclaimed Fossil Sport Collection</u></a></li>
<li><a href="https://buynow-help.techidaily.com/the-ultimate-analysis-of-budget-android-phones-spotlight-on-samsung-galaxy-a20/"><u>The Ultimate Analysis of Budget Android Phones: Spotlight on Samsung Galaxy A20</u></a></li>
<li><a href="https://buynow-help.techidaily.com/the-ultimate-guide-to-the-lenovo-thinkpad-x1-groovyx12-tablet-hybrid-exceptional-portability-quality-2-in-1-function-and-unparalleled-typing-experience/"><u>The Ultimate Guide to the Lenovo ThinkPad X1 groovyX12 Tablet Hybrid – Exceptional Portability, Quality 2-in-1 Function, and Unparalleled Typing Experience</u></a></li>
</ul></div>

