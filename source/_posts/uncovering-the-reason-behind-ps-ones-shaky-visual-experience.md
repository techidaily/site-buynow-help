---
title: Uncovering the Reason Behind PS One's Shaky Visual Experience
date: 2025-01-12T18:20:03.670Z
updated: 2025-01-16T03:20:39.761Z
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/XS1nQCe95LU?si=A2dhdFkSAI61_nKA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

### Highlights

* PlayStation 1 lacked FLOPs due to not having an FPU.
* No Z-buffer resulted in small errors & visible polygons.
* Affine texture mapping caused warping; PS1 trade-offs were speed and cost over complexity.

 Call me biased, but the original PlayStation is still my favorite console of all time. While the games might look a little rough now, they're still as good to play as ever. That said, even back then, PS1 graphics had this signature wobble you didn't find in the competition, so what gives?

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/LI9nKlbhnw8?si=uUXFVbuEqXtFHHv0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  It’s All About Floating Points

 Modern GPU performance is often measured ([controversially](https://hardware-help.techidaily.com/brother-hl-2280dw-driver-package-universal-download-for-windows-11-windows-10-windows-8-and-7-users/)) in FLOPs or FLoating Point Operations. This is simply math involving floating point numbers, which in turn are simply whole numbers with a decimal point. The PlayStation's graphics processor had zero FLOPs, because it lacked an FPU or Floating Point Unit. Instead, it uses fixed-point integers to calculate the positions of vertices.

 A "vertice" is a point where two or more lines meet. So in a polygon, which is typically (but not always) a triangle in 3D graphics, there are three vertices. A 3D model consists of multiple polygons, and as that object moves on screen, the positions of the vertices must be calculated in 3D space.

 Since you can only use integers, any position for a vertice that's not an integer will simply be skipped over. So you'll see polygons "snap" between positions with certain types of motion. For example, a character that's standing still and has a subtle idle animation will look like they're jittering a little.

##  Z-Buffer Not Found

 Apart from the lack of an FPU, the PlayStation also lacked a hardware Z-buffer. You might remember XYZ coordinates from school, where you can describe any point within a 3D space using three numbers. The PlayStation lacked a hardware buffer to store depth or Z-axis values, sorted in order of how far away something is from the "camera."

 This meant that game developers had to create their own in-house Z-buffering solution, and since it was not done in hardware, they had to be economical with their depth-sorting algorithms. This led to a common situation in PS1 games where small sorting errors were made and polygons that should have been hidden from view pop in and out of sight.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/sn2STvYRVb8?si=Z-XhJJ1Mc-Em5Kqy" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Affine Texture Mapping Is Not So Fine After All

 Texture mapping is the process of adding textures (which are basically digital pictures) to a polygon wireframe. It's basically the "skin" of a 3D object. The PS1 uses a method known as "affine" texture mapping, which uses simple math to determine the coordinates on the polygon where the texture should be drawn. Affine texture mapping does not take Z-coordinates into account, and so perspective projection will appear incorrect for 3D objects. Remember the PS1 has no Z-buffer!

 Consoles like the Nintendo 64 do have a Z-buffer, and also use a method known as mipmapping, where multiple versions of a texture are swapped out depending on your distance from the object, further improving the clarity and stability of textures in motion. On the PS1, lacking these technologies, it leads to what's known as affine texture warping.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/K7fATC_lI7o?si=UFotPJqflDRZr-mv" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Fast, Cheap, or Complex: Pick Two

 Different developers did find ways to work around these limitations, and so some PS1 games exhibit these issues to varying degrees. However, trying to address these issues in software almost always means eating up processing power that could have gone to something else. Despite these cutbacks, the PS1's hardware was above all fast. It could pump out polygons faster than anything else at the time.

 It also helps that CRT displays mask most of these issues quite well, and that would have been what the console was designed for. Modern flat panel displays have a negative effect on how PS1 games are presented, making the graphics uglier now than they were back then!

 The bottom line is that the console could have had that extra hardware, but it would have driven the cost up significantly, without any clear benefit to Sony or its players at the time. The company went with "fast and cheap," leaving complexity at the door. History has shown this was the right decision.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/hXIq2G0nShk?si=5Z4Fwv7ZB6oKWsdd" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://fox-http.techidaily.com/new-photovideo-text-warping-essentials-for-2024/"><u>[New] Photo/Video Text Warping Essentials for 2024</u></a></li>
<li><a href="https://youtube-tips.techidaily.com/ransform-your-vision-youtubes-innovative-green-screen-solutions-for-2024/"><u>[New] Transform Your Vision – YouTube's Innovative Green Screen Solutions for 2024</u></a></li>
<li><a href="https://screen-activity-recording.techidaily.com/updated-2024-approved-exceptional-hd-video-capturing-options-compiled-here/"><u>[Updated] 2024 Approved Exceptional HD Video Capturing Options Compiled Here</u></a></li>
<li><a href="https://desktop-recording.techidaily.com/updated-2024-approved-ideal-microphone-logging-software-on-mac-devices-compile-the-best-5/"><u>[Updated] 2024 Approved Ideal Microphone Logging Software on Mac Devices Compile the Best 5</u></a></li>
<li><a href="https://vp-tips.techidaily.com/updated-elite-6-software-for-audiovisual-translation/"><u>[Updated] Elite 6 Software for Audio/Visual Translation</u></a></li>
<li><a href="https://vp-tips.techidaily.com/updated-innovative-editions-filmmaker-writers-on-windows/"><u>[Updated] Innovative Editions Filmmaker' Writers on WIndows</u></a></li>
<li><a href="https://buynow-help.techidaily.com/budget-friendly-radar-detector-reviews-with-the-passport-brand-heres-what-you-need-to-know/"><u>Budget-Friendly Radar Detector Reviews with the Passport Brand, Here's What You Need to Know!</u></a></li>
<li><a href="https://win-blog.techidaily.com/fixing-the-crash-problem-a-step-by-step-solution-for-slime-rancher-2-pc-glitches/"><u>Fixing the Crash Problem: A Step-by-Step Solution for 'Slime Rancher 2' PC Glitches</u></a></li>
<li><a href="https://some-techniques.techidaily.com/harmonizing-your-device-importing-to-inshot-app-for-2024/"><u>Harmonizing Your Device Importing to InShot App for 2024</u></a></li>
<li><a href="https://buynow-help.techidaily.com/hp-notebook-15-review-can-hewlett-packards-budget-priced-amd-laptop-get-the-job-done/"><u>HP Notebook 15 Review: Can Hewlett-Packard’s Budget-Priced AMD Laptop Get the Job Done?</u></a></li>
<li><a href="https://screen-video-capture.techidaily.com/in-2024-capture-and-share-top-no-cost-screen-recorders-for-windowsmac-users/"><u>In 2024, Capture and Share - Top No-Cost Screen Recorders for Windows/Mac Users</u></a></li>
<li><a href="https://buynow-help.techidaily.com/in-depth-appraisal-of-the-compact-yet-resilient-j5-tactical-flashlight-v1-pro/"><u>In Depth Appraisal of the Compact yet Resilient J5 Tactical Flashlight V1-Pro</u></a></li>
<li><a href="https://buynow-help.techidaily.com/samsung-galaxy-fit-evaluation-the-perfect-tracker-for-fitness-enthusiasts/"><u>Samsung Galaxy Fit Evaluation: The Perfect Tracker for Fitness Enthusiasts</u></a></li>
<li><a href="https://buynow-help.techidaily.com/the-motorola-one-hyper-phenomenon-how-this-mid-range-phone-delivers-top-notch-performance-and-style/"><u>The Motorola One Hyper Phenomenon: How This Mid-Range Phone Delivers Top-Notch Performance and Style</u></a></li>
</ul></div>

