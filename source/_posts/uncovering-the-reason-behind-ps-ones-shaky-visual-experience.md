---
title: Uncovering the Reason Behind PS One's Shaky Visual Experience
date: 2024-08-31T12:14:37.086Z
updated: 2024-09-01T12:14:37.086Z
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
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4742929&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/e09fdffe648a30658a9657bbed7b2388/products/boxshot(2).png" border="0">Kanto Player Professional</a>
<!-- affiliate ads end -->
##  Z-Buffer Not Found

 Apart from the lack of an FPU, the PlayStation also lacked a hardware Z-buffer. You might remember XYZ coordinates from school, where you can describe any point within a 3D space using three numbers. The PlayStation lacked a hardware buffer to store depth or Z-axis values, sorted in order of how far away something is from the "camera."

 This meant that game developers had to create their own in-house Z-buffering solution, and since it was not done in hardware, they had to be economical with their depth-sorting algorithms. This led to a common situation in PS1 games where small sorting errors were made and polygons that should have been hidden from view pop in and out of sight.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=45152835&QTY=1&AFFILIATE=108875&CART=1"><img src="https://download.terabyteunlimited.com/banners/ad_800x450_d.jpg" border="0"></a>
<!-- affiliate ads end -->
##  Affine Texture Mapping Is Not So Fine After All

 Texture mapping is the process of adding textures (which are basically digital pictures) to a polygon wireframe. It's basically the "skin" of a 3D object. The PS1 uses a method known as "affine" texture mapping, which uses simple math to determine the coordinates on the polygon where the texture should be drawn. Affine texture mapping does not take Z-coordinates into account, and so perspective projection will appear incorrect for 3D objects. Remember the PS1 has no Z-buffer!

 Consoles like the Nintendo 64 do have a Z-buffer, and also use a method known as mipmapping, where multiple versions of a texture are swapped out depending on your distance from the object, further improving the clarity and stability of textures in motion. On the PS1, lacking these technologies, it leads to what's known as affine texture warping.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4715391&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/7f687767ccf20fcea1c9dc4a5adc2326/Digisigner_banner_728_x_90_color_version.png" border="0"></a>
<!-- affiliate ads end -->
##  Fast, Cheap, or Complex: Pick Two

 Different developers did find ways to work around these limitations, and so some PS1 games exhibit these issues to varying degrees. However, trying to address these issues in software almost always means eating up processing power that could have gone to something else. Despite these cutbacks, the PS1's hardware was above all fast. It could pump out polygons faster than anything else at the time.

 It also helps that CRT displays mask most of these issues quite well, and that would have been what the console was designed for. Modern flat panel displays have a negative effect on how PS1 games are presented, making the graphics uglier now than they were back then!

 The bottom line is that the console could have had that extra hardware, but it would have driven the cost up significantly, without any clear benefit to Sony or its players at the time. The company went with "fast and cheap," leaving complexity at the door. History has shown this was the right decision.

<!-- affiliate ads begin -->
<a href="https://uperfect.sjv.io/c/5597632/1246754/15155" target="_top" id="1246754"><img src="//a.impactradius-go.com/display-ad/15155-1246754" border="0" alt="" width="600" height="600"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1246754/15155" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
##  Emulators Can Correct This (But Should You?)

![An iPad running G-Police next a  physical original copy of the game and a PS4 controller](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/an-ipad-running-g-police-next-a-physical-original-copy-of-the-game-and-a-ps4-controller.jpeg) 

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4721564&QTY=1&AFFILIATE=108875&CART=1">Power Tools add-on for Google Sheets, 12-month subscription</a>
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
<li><a href="https://screen-capture.techidaily.com/new-2024-approved-secure-your-conversations-mastering-free-and-paid-skype-captures-on-pcsmac/"><u>[New] 2024 Approved  Secure Your Conversations  Mastering Free and Paid Skype Captures on PCs/Mac</u></a></li>
<li><a href="https://fox-glue.techidaily.com/new-2024-approved-top-picks-for-shining-3d-type-designs-with-a-golden-touch/"><u>[New] 2024 Approved  Top Picks for Shining 3D Type Designs with a Golden Touch</u></a></li>
<li><a href="https://vp-tips.techidaily.com/new-lgs-virtual-frontier-a-comprehensive-vr-review-for-2024/"><u>[New] LG's Virtual Frontier  A Comprehensive VR Review for 2024</u></a></li>
<li><a href="https://fox-blue.techidaily.com/2024-approved-dji-aerial-lineup-standard-drone-professional-edition-4k-quality/"><u>2024 Approved  DJI Aerial Lineup  Standard Drone, Professional Edition, 4K Quality</u></a></li>
<li><a href="https://extra-support.techidaily.com/2024-approved-mastering-network-live-broadcasts-via-vlc/"><u>2024 Approved  Mastering Network Live Broadcasts via VLC</u></a></li>
<li><a href="https://extra-approaches.techidaily.com/2024-approved-podcasters-soundboard-10-incredible-places-to-find-your-opening-tune/"><u>2024 Approved  Podcaster's Soundboard  10 Incredible Places to Find Your Opening Tune</u></a></li>
<li><a href="https://buynow-help.techidaily.com/a-users-perspective-review-and-recommendations-for-the-anthropics-smart-photo-editor/"><u>A User’s Perspective: Review and Recommendations for the Anthropics Smart Photo Editor</u></a></li>
<li><a href="https://buynow-help.techidaily.com/best-value-and-high-performance-gaming-mini-computers-reviewed/"><u>Best Value and High-Performance Gaming Mini Computers Reviewed</u></a></li>
<li><a href="https://unlock-android.techidaily.com/can-i-bypass-a-forgotten-phone-password-of-xiaomi-13t-pro-by-drfone-android/"><u>Can I Bypass a Forgotten Phone Password Of Xiaomi 13T Pro?</u></a></li>
<li><a href="https://buynow-help.techidaily.com/compact-but-mighty-the-razer-book-13-unleashed-ultimate-gaming-notebook-reviewed/"><u>Compact but Mighty: The Razer Book 13 Unleashed - Ultimate Gaming Notebook Reviewed</u></a></li>
<li><a href="https://buynow-help.techidaily.com/comprehensive-eero-pro-mesh-network-review-ultimate-wireless-solution-for-whole-house-connectivity/"><u>Comprehensive Eero Pro Mesh Network Review: Ultimate Wireless Solution for Whole House Connectivity</u></a></li>
<li><a href="https://buynow-help.techidaily.com/critical-review-of-imperator-rome-conquering-empires-and-overcoming-great-risks/"><u>Critical Review of 'Imperator: Rome' - Conquering Empires and Overcoming Great Risks</u></a></li>
<li><a href="https://buynow-help.techidaily.com/discover-the-best-of-technology-advanced-dell-monitor-anc-audio-experience-and-high-definition-webcam-setup/"><u>Discover the Best of Technology: Advanced Dell Monitor, ANC Audio Experience, and High-Definition Webcam Setup</u></a></li>
<li><a href="https://buynow-help.techidaily.com/discovering-analog-bliss-with-at-lp60xbt/"><u>Discovering Analog Bliss with AT-LP60XBT</u></a></li>
<li><a href="https://buynow-help.techidaily.com/elite-sound-enhancements-best-headphones-for-televisions/"><u>Elite Sound Enhancements: Best Headphones for Televisions</u></a></li>
<li><a href="https://buynow-help.techidaily.com/experience-comfortable-reading-with-budget-friendly-2019-amazon-kindle-model/"><u>Experience Comfortable Reading with Budget-Friendly 2019 Amazon Kindle Model</u></a></li>
<li><a href="https://buynow-help.techidaily.com/experience-excellence-on-a-budget-with-the-oneplus-nord-n100-reviewed-here/"><u>Experience Excellence on a Budget with The OnePlus Nord N100 Reviewed Here!</u></a></li>
<li><a href="https://buynow-help.techidaily.com/experience-uninterrupted-speed-with-d-link-powerline-2000-a-user-friendly-setup-guide/"><u>Experience Uninterrupted Speed with D-Link Powerline 2000: A User-Friendly Setup Guide</u></a></li>
<li><a href="https://buynow-help.techidaily.com/expert-analysis-of-seatechs-external-blu-ray-drive-with-usb-connectivity-a-comprehensive-performance-evaluation/"><u>Expert Analysis of SeaTech's External Blu-Ray Drive with USB Connectivity: A Comprehensive Performance Evaluation</u></a></li>
<li><a href="https://buynow-help.techidaily.com/expert-insights-on-eero-pro-mesh-setup-the-ultimate-router-choice-for-extensive-home-coverage/"><u>Expert Insights on Eero Pro Mesh Setup: The Ultimate Router Choice for Extensive Home Coverage</u></a></li>
<li><a href="https://buynow-help.techidaily.com/expert-reveal-on-twelve-souths-compass-pro-gear-for-optimal-balance-and-control/"><u>Expert Reveal on Twelve South's Compass Pro Gear for Optimal Balance & Control</u></a></li>
<li><a href="https://buynow-help.techidaily.com/exploring-affordability-and-performance-the-samsung-galaxy-a20s-place-among-budget-android-phones/"><u>Exploring Affordability and Performance: The Samsung Galaxy A20's Place Among Budget Android Phones</u></a></li>
<li><a href="https://buynow-help.techidaily.com/exploring-enjoyment-in-pokemon-diamond-and-pokemon-pearl-a-guide/"><u>Exploring Enjoyment in 'Pokémon Diamond & Pokémon Pearl': A Guide</u></a></li>
<li><a href="https://buynow-help.techidaily.com/exploring-the-features-a-closer-look-at-the-revolutionary-samsung-galaxy-s24-ultra/"><u>Exploring the Features: A Closer Look at the Revolutionary Samsung Galaxy S24 Ultra</u></a></li>
<li><a href="https://buynow-help.techidaily.com/exploring-the-pros-and-cons-of-the-costly-samsung-un65nu8000fxza-smart-television/"><u>Exploring the Pros and Cons of the Costly Samsung UN6^5NU8000FXZA Smart Television</u></a></li>
<li><a href="https://ios-pokemon-go.techidaily.com/in-2024-ultimate-guide-to-catch-the-regional-located-pokemon-for-apple-iphone-11-drfone-by-drfone-virtual-ios/"><u>In 2024, Ultimate Guide to Catch the Regional-Located Pokemon For Apple iPhone 11 | Dr.fone</u></a></li>
<li><a href="https://buynow-help.techidaily.com/in-depth-analysis-of-the-kobo-nia-reader-can-it-match-up-to-the-amazon-kindle-standards/"><u>In-Depth Analysis of the Kobo Nia Reader - Can It Match Up to the Amazon Kindle Standards?</u></a></li>
<li><a href="https://buynow-help.techidaily.com/in-depth-analysis-of-the-samsung-galaxy-tab-s7plus-unleashing-a-luxury-android-experience/"><u>In-Depth Analysis of the Samsung Galaxy Tab S7+: Unleashing a Luxury Android Experience</u></a></li>
<li><a href="https://buynow-help.techidaily.com/iphones-or-samsung-smartphones-making-the-right-purchase-decision/"><u>IPhones or Samsung Smartphones: Making the Right Purchase Decision</u></a></li>
<li><a href="https://buynow-help.techidaily.com/kensun-mobile-pneumatic-inflator-review-proven-quality-for-on-the-go-fixes/"><u>Kensun Mobile Pneumatic Inflator Review: Proven Quality for On-the-Go Fixes</u></a></li>
<li><a href="https://buynow-help.techidaily.com/lenovo-tab-m10-hd-2020-reviewed-affordable-quality-for-efficient-web-surfing-and-media-enjoyment/"><u>Lenovo Tab M10 HD 2020 Reviewed - Affordable Quality for Efficient Web Surfing and Media Enjoyment</u></a></li>
<li><a href="https://win-dash.techidaily.com/maintaining-razer-blade-17-performance-driver-update-instructions-for-various-versions-of-windows-os/"><u>Maintaining Razer Blade 17 Performance: Driver Update Instructions for Various Versions of Windows OS</u></a></li>
<li><a href="https://buynow-help.techidaily.com/oneplus-9-evaluation-numerical-analysis-reveals-room-for-improvement/"><u>OnePlus 9 Evaluation: Numerical Analysis Reveals Room for Improvement</u></a></li>
<li><a href="https://buynow-help.techidaily.com/power-under-glass-the-ultimate-list-of-processor-optimized-tablets-evaluated/"><u>Power Under Glass: The Ultimate List of Processor-Optimized Tablets Evaluated</u></a></li>
<li><a href="https://buynow-help.techidaily.com/should-you-opt-for-chatgpt-plus-here-are-five-compelling-reasons-why/"><u>Should You Opt for ChatGPT Plus? Here Are Five Compelling Reasons Why!</u></a></li>
<li><a href="https://howto.techidaily.com/super-easy-ways-to-deal-with-poco-f5-5g-unresponsive-screen-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>Super Easy Ways To Deal with Poco F5 5G Unresponsive Screen | Dr.fone</u></a></li>
<li><a href="https://buynow-help.techidaily.com/the-truth-about-amazon-luna-is-it-the-ultimate-in-effortless-gaming-experience/"><u>The Truth About Amazon Luna: Is It the Ultimate in Effortless Gaming Experience</u></a></li>
<li><a href="https://buynow-help.techidaily.com/the-ultimate-list-microsoft-office-alternatives-dominating-2024/"><u>The Ultimate List: Microsoft Office Alternatives Dominating 2024</u></a></li>
<li><a href="https://buynow-help.techidaily.com/top-rated-gimp-the-ultimate-no-cost-cross-os-image-editing-software-examined/"><u>Top Rated GIMP: The Ultimate No-Cost, Cross-OS Image Editing Software Examined</u></a></li>
<li><a href="https://buynow-help.techidaily.com/top-rated-mouse-options-for-your-ipad-find-the-perfect-match/"><u>Top-Rated Mouse Options for Your iPad: Find the Perfect Match</u></a></li>
<li><a href="https://buynow-help.techidaily.com/unveiling-the-benefits-of-ergodrivens-topo-anti-fatigue-mat-a-comprehensive-review-for-standing-desks-enthusiasts/"><u>Unveiling the Benefits of ErgoDriven's Topo Anti-Fatigue Mat - A Comprehensive Review for Standing Desks Enthusiasts</u></a></li>
<li><a href="https://buynow-help.techidaily.com/unveiling-the-power-of-the-fitbit-versa-2-a-wearable-that-elevates-your-health-game-and-offers-cutting-edge-smartwatch-extras/"><u>Unveiling the Power of the Fitbit Versa 2 - A Wearable that Elevates Your Health Game and Offers Cutting-Edge Smartwatch Extras</u></a></li>
</ul></div>
