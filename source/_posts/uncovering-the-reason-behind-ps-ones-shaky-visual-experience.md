---
title: Uncovering the Reason Behind PS One's Shaky Visual Experience
date: 2024-10-21T11:58:37.105Z
updated: 2024-10-23T18:20:35.517Z
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
<a href="https://aligracehair.sjv.io/c/5597632/1938677/19272" target="_top" id="1938677">
  <img src="//a.impactradius-go.com/display-ad/19272-1938677" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1938677/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  It’s All About Floating Points

 Modern GPU performance is often measured ([controversially](https://hardware-help.techidaily.com/brother-hl-2280dw-driver-package-universal-download-for-windows-11-windows-10-windows-8-and-7-users/)) in FLOPs or FLoating Point Operations. This is simply math involving floating point numbers, which in turn are simply whole numbers with a decimal point. The PlayStation's graphics processor had zero FLOPs, because it lacked an FPU or Floating Point Unit. Instead, it uses fixed-point integers to calculate the positions of vertices.

 A "vertice" is a point where two or more lines meet. So in a polygon, which is typically (but not always) a triangle in 3D graphics, there are three vertices. A 3D model consists of multiple polygons, and as that object moves on screen, the positions of the vertices must be calculated in 3D space.

 Since you can only use integers, any position for a vertice that's not an integer will simply be skipped over. So you'll see polygons "snap" between positions with certain types of motion. For example, a character that's standing still and has a subtle idle animation will look like they're jittering a little.

##  Z-Buffer Not Found

 Apart from the lack of an FPU, the PlayStation also lacked a hardware Z-buffer. You might remember XYZ coordinates from school, where you can describe any point within a 3D space using three numbers. The PlayStation lacked a hardware buffer to store depth or Z-axis values, sorted in order of how far away something is from the "camera."

 This meant that game developers had to create their own in-house Z-buffering solution, and since it was not done in hardware, they had to be economical with their depth-sorting algorithms. This led to a common situation in PS1 games where small sorting errors were made and polygons that should have been hidden from view pop in and out of sight.

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2135403/19272" target="_top" id="2135403">
  <img src="//a.impactradius-go.com/display-ad/19272-2135403" border="0" alt="https://techidaily.com" width="392" height="72"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135403/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Affine Texture Mapping Is Not So Fine After All

 Texture mapping is the process of adding textures (which are basically digital pictures) to a polygon wireframe. It's basically the "skin" of a 3D object. The PS1 uses a method known as "affine" texture mapping, which uses simple math to determine the coordinates on the polygon where the texture should be drawn. Affine texture mapping does not take Z-coordinates into account, and so perspective projection will appear incorrect for 3D objects. Remember the PS1 has no Z-buffer!

 Consoles like the Nintendo 64 do have a Z-buffer, and also use a method known as mipmapping, where multiple versions of a texture are swapped out depending on your distance from the object, further improving the clarity and stability of textures in motion. On the PS1, lacking these technologies, it leads to what's known as affine texture warping.

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2135394/19272" target="_top" id="2135394">
  <img src="//a.impactradius-go.com/display-ad/19272-2135394" border="0" alt="https://techidaily.com" width="120" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135394/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Fast, Cheap, or Complex: Pick Two

 Different developers did find ways to work around these limitations, and so some PS1 games exhibit these issues to varying degrees. However, trying to address these issues in software almost always means eating up processing power that could have gone to something else. Despite these cutbacks, the PS1's hardware was above all fast. It could pump out polygons faster than anything else at the time.

 It also helps that CRT displays mask most of these issues quite well, and that would have been what the console was designed for. Modern flat panel displays have a negative effect on how PS1 games are presented, making the graphics uglier now than they were back then!

 The bottom line is that the console could have had that extra hardware, but it would have driven the cost up significantly, without any clear benefit to Sony or its players at the time. The company went with "fast and cheap," leaving complexity at the door. History has shown this was the right decision.

##  Emulators Can Correct This (But Should You?)

![An iPad running G-Police next a  physical original copy of the game and a PS4 controller](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/an-ipad-running-g-police-next-a-physical-original-copy-of-the-game-and-a-ps4-controller.jpeg) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2027176/19272" target="_top" id="2027176">
  <img src="//a.impactradius-go.com/display-ad/19272-2027176" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2027176/19272" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://youtube-tips.techidaily.com/024-approved-maximizing-screen-time-selecting-an-mcn-wisely/"><u>[New] 2024 Approved Maximizing Screen Time Selecting an MCN Wisely</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-iconic-highlights-from-the-2022-figure-skate-world/"><u>[Updated] Iconic Highlights From the 2022 Figure Skate World</u></a></li>
<li><a href="https://visual-screen-recording.techidaily.com/updated-in-2024-optimizing-your-whiteboard-use-on-desktopiosandroid-devices-in-a-zoom-environment/"><u>[Updated] In 2024, Optimizing Your Whiteboard Use on Desktop/iOS/Android Devices in a Zoom Environment</u></a></li>
<li><a href="https://extra-resources.techidaily.com/2024-approved-auditory-ambition-realized-selecting-the-ultimate-interface/"><u>2024 Approved Auditory Ambition Realized Selecting the Ultimate Interface</u></a></li>
<li><a href="https://extra-hints.techidaily.com/2024-approved-build-funny-images-kapwings-meme-studio/"><u>2024 Approved Build Funny Images Kapwing’s Meme Studio</u></a></li>
<li><a href="https://some-skills.techidaily.com/2024-approved-the-ultimate-checklist-for-google-podcast-enthusiasts/"><u>2024 Approved The Ultimate Checklist for Google Podcast Enthusiasts</u></a></li>
<li><a href="https://howto.techidaily.com/7-solutions-to-fix-error-code-963-on-google-play-of-nokia-c32-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>7 Solutions to Fix Error Code 963 on Google Play Of Nokia C32 | Dr.fone</u></a></li>
<li><a href="https://buynow-help.techidaily.com/classic-meets-high-tech-an-in-depth-review-of-the-stylish-skagen-falster-3-smartwatch/"><u>Classic Meets High-Tech: An In-Depth Review of the Stylish Skagen Falster 3 Smartwatch</u></a></li>
<li><a href="https://buynow-help.techidaily.com/create-a-research-budget/"><u>Create a Research Budget:</u></a></li>
<li><a href="https://buynow-help.techidaily.com/explore-the-innovative-features-of-mods-newest-easyside-carrier-ebike-model/"><u>Explore the Innovative Features of Mod's Newest EasySide Carrier eBike Model</u></a></li>
<li><a href="https://win-able.techidaily.com/getting-avatars-latest-expansion-to-boot-on-your-system/"><u>Getting Avatar's Latest Expansion to Boot on Your System?</u></a></li>
<li><a href="https://buynow-help.techidaily.com/revolutionary-convertible-laptop-revealed-the-dell-xps-13-7390-with-exceptional-performance-and-style/"><u>Revolutionary Convertible Laptop Revealed - The Dell XPS 13 7390 with Exceptional Performance and Style</u></a></li>
<li><a href="https://buynow-help.techidaily.com/standing-desk-pad-review-for-ergohead-users-seeking-long-duration-support/"><u>Standing Desk Pad Review for Ergohead Users Seeking Long-Duration Support</u></a></li>
<li><a href="https://buynow-help.techidaily.com/top-reviews-for-samsungs-latest-marvel-the-galaxy-note20-ultra-5g-unveiled/"><u>Top Reviews for Samsung's Latest Marvel - The Galaxy Note20 Ultra 5G Unveiled</u></a></li>
</ul></div>

