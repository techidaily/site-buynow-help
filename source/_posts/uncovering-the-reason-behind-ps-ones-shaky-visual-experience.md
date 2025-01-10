---
title: Uncovering the Reason Behind PS One's Shaky Visual Experience
date: 2025-01-06T20:17:18.874Z
updated: 2025-01-09T19:36:31.552Z
tags:
  - games
  - tv
  - movies
categories:
  - tech
thumbnail: https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/06/a-playstation-1-controller-with-metal-gear-solid-running-on-a-tv-and-a-glitch-effect.jpg
---

## Uncovering the Reason Behind PS One's Shaky Visual Experience

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/Jng92DT1n_Y?si=LvxQhsEJoymsM2iZ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

### Highlights

* PlayStation 1 lacked FLOPs due to not having an FPU.
* No Z-buffer resulted in small errors & visible polygons.
* Affine texture mapping caused warping; PS1 trade-offs were speed and cost over complexity.

 Call me biased, but the original PlayStation is still my favorite console of all time. While the games might look a little rough now, they're still as good to play as ever. That said, even back then, PS1 graphics had this signature wobble you didn't find in the competition, so what gives?

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/PKZUYice-ws?si=L8iMa9T3h7TMSWdQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  It’s All About Floating Points

 Modern GPU performance is often measured ([controversially](https://hardware-help.techidaily.com/brother-hl-2280dw-driver-package-universal-download-for-windows-11-windows-10-windows-8-and-7-users/)) in FLOPs or FLoating Point Operations. This is simply math involving floating point numbers, which in turn are simply whole numbers with a decimal point. The PlayStation's graphics processor had zero FLOPs, because it lacked an FPU or Floating Point Unit. Instead, it uses fixed-point integers to calculate the positions of vertices.

 A "vertice" is a point where two or more lines meet. So in a polygon, which is typically (but not always) a triangle in 3D graphics, there are three vertices. A 3D model consists of multiple polygons, and as that object moves on screen, the positions of the vertices must be calculated in 3D space.

 Since you can only use integers, any position for a vertice that's not an integer will simply be skipped over. So you'll see polygons "snap" between positions with certain types of motion. For example, a character that's standing still and has a subtle idle animation will look like they're jittering a little.

##  Z-Buffer Not Found

 Apart from the lack of an FPU, the PlayStation also lacked a hardware Z-buffer. You might remember XYZ coordinates from school, where you can describe any point within a 3D space using three numbers. The PlayStation lacked a hardware buffer to store depth or Z-axis values, sorted in order of how far away something is from the "camera."

 This meant that game developers had to create their own in-house Z-buffering solution, and since it was not done in hardware, they had to be economical with their depth-sorting algorithms. This led to a common situation in PS1 games where small sorting errors were made and polygons that should have been hidden from view pop in and out of sight.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/JAkb8Bv3AU4?si=2rHwnZYTzTLieKgY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Affine Texture Mapping Is Not So Fine After All

 Texture mapping is the process of adding textures (which are basically digital pictures) to a polygon wireframe. It's basically the "skin" of a 3D object. The PS1 uses a method known as "affine" texture mapping, which uses simple math to determine the coordinates on the polygon where the texture should be drawn. Affine texture mapping does not take Z-coordinates into account, and so perspective projection will appear incorrect for 3D objects. Remember the PS1 has no Z-buffer!

 Consoles like the Nintendo 64 do have a Z-buffer, and also use a method known as mipmapping, where multiple versions of a texture are swapped out depending on your distance from the object, further improving the clarity and stability of textures in motion. On the PS1, lacking these technologies, it leads to what's known as affine texture warping.

##  Fast, Cheap, or Complex: Pick Two

 Different developers did find ways to work around these limitations, and so some PS1 games exhibit these issues to varying degrees. However, trying to address these issues in software almost always means eating up processing power that could have gone to something else. Despite these cutbacks, the PS1's hardware was above all fast. It could pump out polygons faster than anything else at the time.

 It also helps that CRT displays mask most of these issues quite well, and that would have been what the console was designed for. Modern flat panel displays have a negative effect on how PS1 games are presented, making the graphics uglier now than they were back then!

 The bottom line is that the console could have had that extra hardware, but it would have driven the cost up significantly, without any clear benefit to Sony or its players at the time. The company went with "fast and cheap," leaving complexity at the door. History has shown this was the right decision.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/K4lRBnNnd9k?si=5e0MbdOz-fF6Ry_k" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Emulators Can Correct This (But Should You?)

![An iPad running G-Police next a  physical original copy of the game and a PS4 controller](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/an-ipad-running-g-police-next-a-physical-original-copy-of-the-game-and-a-ps4-controller.jpeg) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/mK1lEBRm_1w?si=FSaM0OKO0XBCgjtT" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://youtube-webster.techidaily.com/024-approved-unlock-youtube-placement-secrets-what-matters-most/"><u>[New] 2024 Approved Unlock YouTube Placement Secrets What Matters Most?</u></a></li>
<li><a href="https://extra-hints.techidaily.com/updated-best-of-breed-exceptional-cardboard-vr-gaming-experienits/"><u>[Updated] Best of Breed Exceptional Cardboard VR Gaming Experienits</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/2024-approved-imaginarium-collagecraft-cutting-edge-assembler/"><u>2024 Approved Imaginarium CollageCraft Cutting-Edge Assembler</u></a></li>
<li><a href="https://technical-tips.techidaily.com/en-ligne-pour-toute-la-journee-convertissez-votre-musique-gsm-au-format-mp3-avec-le-convertisseur-gratuit-de-movavi/"><u>En Ligne Pour Toute La Journée : Convertissez Votre Musique GSM Au Format MP3 Avec Le Convertisseur Gratuit De Movavi</u></a></li>
<li><a href="https://fox-access.techidaily.com/freelance-warriors-guide-complimentary-psd-treasures/"><u>Freelance Warriors Guide Complimentary PSD Treasures</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/in-2024-how-to-use-allshare-cast-to-turn-on-screen-mirroring-on-samsung-galaxy-a15-5g-drfone-by-drfone-android/"><u>In 2024, How To Use Allshare Cast To Turn On Screen Mirroring On Samsung Galaxy A15 5G | Dr.fone</u></a></li>
<li><a href="https://buynow-help.techidaily.com/ps5-versus-ps5-slim-understanding-the-key-distinctions-between-models/"><u>PS5 Versus PS5 Slim – Understanding the Key Distinctions Between Models</u></a></li>
<li><a href="https://buynow-help.techidaily.com/scosche-revolt-dual-review/"><u>Scosche ReVolt Dual Review</u></a></li>
<li><a href="https://win-tutorials.techidaily.com/step-by-step-guide-to-retrieving-accidentally-erased-files-from-usb-memory-sticks-for-free/"><u>Step-by-Step Guide to Retrieving Accidentally Erased Files From USB Memory Sticks for Free</u></a></li>
<li><a href="https://blog-min.techidaily.com/step-by-step-guide-transferring-data-from-your-iphone-to-a-mac-without-using-itunes-or-icloud/"><u>Step-by-Step Guide: Transferring Data From Your iPhone to a Mac Without Using iTunes or iCloud</u></a></li>
<li><a href="https://buynow-help.techidaily.com/the-enigmatic-identity-of-microsoft-surface-go-unveiled-in-our-affordable-tablet-review/"><u>The Enigmatic Identity of Microsoft Surface Go Unveiled in Our Affordable Tablet Review</u></a></li>
<li><a href="https://buynow-help.techidaily.com/the-ultimate-companer-for-on-the-go-power-an-extensive-review-of-maxoaks-185wh50000mah-bank/"><u>The Ultimate Companer for On-the-Go Power: An Extensive Review of MaxOak's 185Wh/50000mAh Bank</u></a></li>
<li><a href="https://buynow-help.techidaily.com/the-ultimate-guide-to-choosing-fongo-in-canada-exploring-superior-voip-services-for-business-and-personal-use/"><u>The Ultimate Guide to Choosing Fongo in Canada: Exploring Superior VoIP Services for Business and Personal Use</u></a></li>
<li><a href="https://unlock-android.techidaily.com/top-4-sim-location-trackers-to-easily-find-your-lost-vivo-v30-device-by-drfone-android/"><u>Top 4 SIM Location Trackers To Easily Find Your Lost Vivo V30 Device</u></a></li>
<li><a href="https://buynow-help.techidaily.com/top-acer-savings-on-prime-day-2024-unbeatable-offers/"><u>Top Acer Savings on Prime Day 2024: Unbeatable Offers!</u></a></li>
<li><a href="https://buynow-help.techidaily.com/top-showdown-how-does-apple-tv-4k-stack-up-against-roku-ultra-in-a-side-by-side-comparison/"><u>Top Showdown: How Does Apple TV 4K Stack Up Against Roku Ultra in a Side-by-Side Comparison?</u></a></li>
<li><a href="https://buynow-help.techidaily.com/top-tier-performance-with-ibuypowers-high-value-gaming-rig-in-depth-review/"><u>Top-Tier Performance with IBUYPOWER's High-Value Gaming Rig - In-Depth Review</u></a></li>
<li><a href="https://tech-revival.techidaily.com/ultimate-guide-to-editing-obs-videos-without-a-watermark-top-7-tools-compared/"><u>Ultimate Guide to Editing OBS Videos without a Watermark – Top 7 Tools Compared</u></a></li>
<li><a href="https://buynow-help.techidaily.com/unboxing-sonys-xperia-5-size-and-price-overview/"><u>Unboxing Sony's Xperia 5: Size and Price Overview</u></a></li>
</ul></div>

