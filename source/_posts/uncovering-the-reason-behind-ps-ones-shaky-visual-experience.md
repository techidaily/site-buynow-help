---
title: Uncovering the Reason Behind PS One's Shaky Visual Experience
date: 2024-10-29T06:21:32.451Z
updated: 2024-10-29T23:11:50.926Z
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
<span id="701707">
					<video width="1536" height="864" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/701707.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/7443-701707">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/701707.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:960px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fappsumo.8odi.net%2Fc%2F5597632%2F701707%2F7443'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/701707/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Z-Buffer Not Found

 Apart from the lack of an FPU, the PlayStation also lacked a hardware Z-buffer. You might remember XYZ coordinates from school, where you can describe any point within a 3D space using three numbers. The PlayStation lacked a hardware buffer to store depth or Z-axis values, sorted in order of how far away something is from the "camera."

 This meant that game developers had to create their own in-house Z-buffering solution, and since it was not done in hardware, they had to be economical with their depth-sorting algorithms. This led to a common situation in PS1 games where small sorting errors were made and polygons that should have been hidden from view pop in and out of sight.

<!-- affiliate ads begin -->
<a href="https://aidotcom.pxf.io/c/5597632/2134499/19576" target="_top" id="2134499">
  <img src="//a.impactradius-go.com/display-ad/19576-2134499" border="0" alt="https://techidaily.com" width="600" height="90"/>
</a>
<img height="0" width="0" src="https://aidotcom.pxf.io/i/5597632/2134499/19576" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Affine Texture Mapping Is Not So Fine After All

 Texture mapping is the process of adding textures (which are basically digital pictures) to a polygon wireframe. It's basically the "skin" of a 3D object. The PS1 uses a method known as "affine" texture mapping, which uses simple math to determine the coordinates on the polygon where the texture should be drawn. Affine texture mapping does not take Z-coordinates into account, and so perspective projection will appear incorrect for 3D objects. Remember the PS1 has no Z-buffer!

 Consoles like the Nintendo 64 do have a Z-buffer, and also use a method known as mipmapping, where multiple versions of a texture are swapped out depending on your distance from the object, further improving the clarity and stability of textures in motion. On the PS1, lacking these technologies, it leads to what's known as affine texture warping.

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1975802/19272" target="_top" id="1975802">
  <img src="//a.impactradius-go.com/display-ad/19272-1975802" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1975802/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Fast, Cheap, or Complex: Pick Two

 Different developers did find ways to work around these limitations, and so some PS1 games exhibit these issues to varying degrees. However, trying to address these issues in software almost always means eating up processing power that could have gone to something else. Despite these cutbacks, the PS1's hardware was above all fast. It could pump out polygons faster than anything else at the time.

 It also helps that CRT displays mask most of these issues quite well, and that would have been what the console was designed for. Modern flat panel displays have a negative effect on how PS1 games are presented, making the graphics uglier now than they were back then!

 The bottom line is that the console could have had that extra hardware, but it would have driven the cost up significantly, without any clear benefit to Sony or its players at the time. The company went with "fast and cheap," leaving complexity at the door. History has shown this was the right decision.

##  Emulators Can Correct This (But Should You?)

![An iPad running G-Police next a  physical original copy of the game and a PS4 controller](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/an-ipad-running-g-police-next-a-physical-original-copy-of-the-game-and-a-ps4-controller.jpeg) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2100527/7443" target="_top" id="2100527">
  <img src="//a.impactradius-go.com/display-ad/7443-2100527" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2100527/7443" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://tiktok-clips.techidaily.com/updated-hot-off-the-internet-discover-amazons-30-tiktok-must-haves/"><u>[Updated] Hot Off the Internet? Discover Amazon's 30 TikTok Must-Haves</u></a></li>
<li><a href="https://youtube-blog.techidaily.com/ed-visionary-voices-celebrating-innovative-female-creators-on-youtube/"><u>[Updated] Visionary Voices Celebrating Innovative Female Creators on YouTube</u></a></li>
<li><a href="https://extra-tips.techidaily.com/2024-approved-affordable-cameras-where-to-buy-economical-gopros/"><u>2024 Approved Affordable Cameras Where to Buy Economical GoPros</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/2024-approved-high-resolution-drone-flights-a-mi-examination/"><u>2024 Approved High-Resolution Drone Flights A MI Examination</u></a></li>
<li><a href="https://fox-direct.techidaily.com/2024-approved-starting-with-simple-tricks-auditions-fade-techniques/"><u>2024 Approved Starting with Simple Tricks Audition's Fade Techniques</u></a></li>
<li><a href="https://win-great.techidaily.com/1728491158342-windows-10/"><u>完全なWindows 10オペレーティングシステムを保護するためのガイド</u></a></li>
<li><a href="https://technical-tips.techidaily.com/desktop-users-rejoice-enabling-snapchat-on-your-laptop-easily/"><u>Desktop Users Rejoice: Enabling Snapchat on Your Laptop Easily!</u></a></li>
<li><a href="https://buynow-help.techidaily.com/expert-insights-on-the-sleek-and-efficient-anker-powercoreplus-26800-charger-combo-review/"><u>Expert Insights on the Sleek and Efficient Anker PowerCore+ 26800 Charger Combo Review</u></a></li>
<li><a href="https://android-unlock.techidaily.com/in-2024-how-to-change-samsung-galaxy-f54-5g-lock-screen-password-by-drfone-android/"><u>In 2024, How To Change Samsung Galaxy F54 5G Lock Screen Password?</u></a></li>
<li><a href="https://buynow-help.techidaily.com/insights-and-opinions-on-the-updated-apple-books-mobile-application/"><u>Insights and Opinions on the Updated Apple Books Mobile Application</u></a></li>
<li><a href="https://buynow-help.techidaily.com/nokia-71-phone-analysis-stunning-display-and-photography-at-an-exceptional-value/"><u>Nokia 7.1 Phone Analysis - Stunning Display & Photography at an Exceptional Value</u></a></li>
<li><a href="https://buynow-help.techidaily.com/top-rated-acer-aspire-e-15-the-ultimate-guide-to-affordable-power/"><u>Top-Rated Acer Aspire E 15: The Ultimate Guide to Affordable Power</u></a></li>
<li><a href="https://buynow-help.techidaily.com/unlocking-ultra-hd-entertainment-with-amazons-insignia-ns-43df710na19-fire-tv-stick-an-insightful-and-affordable-option/"><u>Unlocking Ultra HD Entertainment with Amazon's Insignia NS-43DF710NA19 Fire TV Stick: An Insightful and Affordable Option</u></a></li>
<li><a href="https://buynow-help.techidaily.com/unveiling-the-performance-and-capabilities-of-the-newly-released-google-pixel-6-phone/"><u>Unveiling the Performance and Capabilities of the Newly Released Google Pixel 6 Phone</u></a></li>
<li><a href="https://fox-shield.techidaily.com/1728478203555-windows-11/"><u>Windows 11で最適化された増分・差分バックアップガイド</u></a></li>
<li><a href="https://buynow-help.techidaily.com/xiaomi-mi-smart-band-4-evaluation-how-it-outshines-budget-competitors-in-fitness-tracking/"><u>Xiaomi Mi Smart Band 4 Evaluation: How It Outshines Budget Competitors in Fitness Tracking</u></a></li>
</ul></div>

