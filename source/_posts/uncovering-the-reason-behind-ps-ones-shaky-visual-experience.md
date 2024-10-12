---
title: Uncovering the Reason Behind PS One's Shaky Visual Experience
date: 2024-10-05T18:05:05.360Z
updated: 2024-10-12T18:23:39.219Z
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

<!-- affiliate ads begin -->
<a href="https://unicoeye.pxf.io/c/5597632/2148773/18498" target="_top" id="2148773">
  <img src="//a.impactradius-go.com/display-ad/18498-2148773" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://unicoeye.pxf.io/i/5597632/2148773/18498" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Affine Texture Mapping Is Not So Fine After All

 Texture mapping is the process of adding textures (which are basically digital pictures) to a polygon wireframe. It's basically the "skin" of a 3D object. The PS1 uses a method known as "affine" texture mapping, which uses simple math to determine the coordinates on the polygon where the texture should be drawn. Affine texture mapping does not take Z-coordinates into account, and so perspective projection will appear incorrect for 3D objects. Remember the PS1 has no Z-buffer!

 Consoles like the Nintendo 64 do have a Z-buffer, and also use a method known as mipmapping, where multiple versions of a texture are swapped out depending on your distance from the object, further improving the clarity and stability of textures in motion. On the PS1, lacking these technologies, it leads to what's known as affine texture warping.

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1997662/19272" target="_top" id="1997662">
  <img src="//a.impactradius-go.com/display-ad/19272-1997662" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1997662/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Fast, Cheap, or Complex: Pick Two

 Different developers did find ways to work around these limitations, and so some PS1 games exhibit these issues to varying degrees. However, trying to address these issues in software almost always means eating up processing power that could have gone to something else. Despite these cutbacks, the PS1's hardware was above all fast. It could pump out polygons faster than anything else at the time.

 It also helps that CRT displays mask most of these issues quite well, and that would have been what the console was designed for. Modern flat panel displays have a negative effect on how PS1 games are presented, making the graphics uglier now than they were back then!

 The bottom line is that the console could have had that extra hardware, but it would have driven the cost up significantly, without any clear benefit to Sony or its players at the time. The company went with "fast and cheap," leaving complexity at the door. History has shown this was the right decision.

<!-- affiliate ads begin -->
<a href="https://25home.pxf.io/c/5597632/2148646/16836" target="_top" id="2148646">
  <img src="//a.impactradius-go.com/display-ad/16836-2148646" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://25home.pxf.io/i/5597632/2148646/16836" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Emulators Can Correct This (But Should You?)

![An iPad running G-Police next a  physical original copy of the game and a PS4 controller](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/an-ipad-running-g-police-next-a-physical-original-copy-of-the-game-and-a-ps4-controller.jpeg) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2037474/7443" target="_top" id="2037474">
  <img src="//a.impactradius-go.com/display-ad/7443-2037474" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2037474/7443" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://screen-capture.techidaily.com/new-convert-and-store-webcam-footage-in-vlc-media-for-2024/"><u>[New] Convert & Store Webcam Footage in VLC Media for 2024</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/new-revolutionizing-your-digital-presence-through-strategic-social-media-mastery/"><u>[New] Revolutionizing Your Digital Presence Through Strategic Social Media Mastery</u></a></li>
<li><a href="https://some-tips.techidaily.com/new-summers-best-10-nostalgic-films-for-the-whole-family/"><u>[New] Summer's Best 10 Nostalgic Films for the Whole Family</u></a></li>
<li><a href="https://article-tips.techidaily.com/updated-2024-approved-lg-bp350-evaluation-size-resolution-and-connectivity/"><u>[Updated] 2024 Approved LG BP350 Evaluation - Size, Resolution, and Connectivity</u></a></li>
<li><a href="https://howto.techidaily.com/9-solutions-to-fix-process-system-isnt-responding-error-on-oppo-find-n3-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>9 Solutions to Fix Process System Isnt Responding Error on Oppo Find N3 | Dr.fone</u></a></li>
<li><a href="https://fox-that.techidaily.com/effortless-solutions-to-common-setbacks-in-using-apple-pay/"><u>Effortless Solutions to Common Setbacks in Using Apple Pay</u></a></li>
<li><a href="https://win-data.techidaily.com/how-to-produce-free-educational-video-guides-easily/"><u>How to Produce Free Educational Video Guides Easily</u></a></li>
<li><a href="https://vimeo-videos.techidaily.com/ideal-video-editor-unleashed-for-vimeo-videos-for-2024/"><u>Ideal Video Editor Unleashed for Vimeo Videos for 2024</u></a></li>
<li><a href="https://unlock-android.techidaily.com/in-2024-how-to-show-wi-fi-password-on-xiaomi-redmi-note-12t-pro-by-drfone-android/"><u>In 2024, How to Show Wi-Fi Password on Xiaomi Redmi Note 12T Pro</u></a></li>
<li><a href="https://buynow-help.techidaily.com/the-definitive-review-of-huaweis-mediapad-m5-a-tablet-revolutionizing-audio-visual-engagement/"><u>The Definitive Review of Huawei's MediaPad M5 - A Tablet Revolutionizing Audio-Visual Engagement</u></a></li>
<li><a href="https://buynow-help.techidaily.com/the-lenovo-thinkpad-x1-fold-unveiled-pioneering-yet-problematic/"><u>The Lenovo ThinkPad X1 Fold Unveiled - Pioneering Yet Problematic</u></a></li>
<li><a href="https://buynow-help.techidaily.com/the-ultimate-guide-to-mastery-of-the-samsung-galaxy-tab-s5e-your-go-to-for-an-advanced-android-tablet-review/"><u>The Ultimate Guide to Mastery of the Samsung Galaxy Tab S^5E: Your Go-To for an Advanced Android Tablet Review</u></a></li>
<li><a href="https://buynow-help.techidaily.com/the-unbeatable-deal-in-laptops-discover-how-acer-aspire-e-15-delivers-top-performance-without-breaking-the-bank/"><u>The Unbeatable Deal in Laptops: Discover How Acer Aspire E 15 Delivers Top Performance Without Breaking the Bank</u></a></li>
<li><a href="https://buynow-help.techidaily.com/top-7-must-see-sites-for-latest-film-previews/"><u>Top 7 Must-See Sites for Latest Film Previews</u></a></li>
<li><a href="https://buynow-help.techidaily.com/top-replacement-options-for-microsoft-office/"><u>Top Replacement Options for Microsoft Office</u></a></li>
<li><a href="https://buynow-help.techidaily.com/unlocking-the-potential-of-virtual-reality-oculus-quest-2-elite-strap-plus-battery-bundle-assessment/"><u>Unlocking the Potential of Virtual Reality: Oculus Quest ^2 Elite Strap + Battery Bundle Assessment</u></a></li>
<li><a href="https://buynow-help.techidaily.com/unveiling-innovation-how-amazon-halo-redefines-comprehensive-health-monitoring-devices/"><u>Unveiling Innovation: How Amazon Halo Redefines Comprehensive Health Monitoring Devices</u></a></li>
<li><a href="https://buynow-help.techidaily.com/unveiling-the-linksys-max-stream-ac1e-networking-solution-ideal-for-wide-audiences/"><u>Unveiling the Linksys Max-Stream AC1e Networking Solution - Ideal for Wide Audiences</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/which-pokemon-can-evolve-with-a-moon-stone-for-tecno-spark-10-5g-drfone-by-drfone-virtual-android/"><u>Which Pokémon can Evolve with a Moon Stone For Tecno Spark 10 5G? | Dr.fone</u></a></li>
</ul></div>

