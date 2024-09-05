---
title: "Understanding JIT: The Impact of Apples Legal Framework on iOS Gaming Emulation"
date: 2024-09-04T16:07:52.499Z
updated: 2024-09-05T16:07:52.499Z
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

##  What Is JIT?

 JIT compilation is short for "Just In Time" compilation. Compilation is the process of turning programming code into machine code. You can write something in, for example, C code and then compile it for any system, whether it's an x86 CPU as found on most Windows computers or an ARM CPU as found on mobile phones and tablets.

 JIT compilation, as opposed to ahead-of-time compilation, has numerous advantages, not least of which is adaptability to what's currently happening on the computer and what the user is asking the program to do.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2082542/7443" target="_top" id="2082542">
  <img src="//a.impactradius-go.com/display-ad/7443-2082542" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2082542/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
##  Why Do Emulators Need JIT?

 The developers of emulators have found that the JIT approach lets them achieve levels of performance and efficiency that would otherwise be impossible. Using the JIT technique, the emulated CPU code from the original system can be recompiled to native code for the target host system on the fly. Once that code has been recompiled, it can be cached and used the next time the same call is made without compiling again.

![An iPad running G-Police next a  physical original copy of the game and a PS4 controller](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/an-ipad-running-g-police-next-a-physical-original-copy-of-the-game-and-a-ps4-controller.jpeg) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2030381/7443" target="_top" id="2030381">
  <img src="//a.impactradius-go.com/display-ad/7443-2030381" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2030381/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
Sydney Louw Butler / How-To Geek

 Using the JIT method, it's possible to create self-modifying code, which has become a common approach in video game emulation. This is necessary in some systems because many older systems, particularly cartridge based systems, would load code from the cartridge dynamically and seemingly arbitrarily based on the exact game state. JIT allows for essentially real-time handling of this approach. JIT also lets the emulator optimize the recompiled code to take advantage of the host system as much as possible.

 I'm not a programmer, but even from my point of view, JIT seems like an extremely powerful tool when applied to the tough problem of emulation, based on what I've read.

<!-- affiliate ads begin -->
<a href="https://imp.i357552.net/c/5597632/947750/11832" target="_top" id="947750">
  <img src="//a.impactradius-go.com/display-ad/11832-947750" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://imp.i357552.net/i/5597632/947750/11832" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
##  Why Doesn't Apple Allow JIT?

 Unfortunately, another type of software that can make great use of JIT and self-modifying code is malware. If an app can generate and execute code during its runtime, that opens up the door to all sorts of shenanigans So compiling all the code ahead of time makes it much easier to ensure that the code is safe. Apple also likely doesn't want to have a situation where an app changes its behavior after being approved. Something which can't happen if the pre-compiled code is static.

 The knock-on effect is that software which relies on a JIT recompiler to work at usable speeds won't be approved for the App Store. This is the reason given for the [absence of the popular Dolphin emulator](https://oatmealdome.me/blog/why-dolphin-isnt-coming-to-the-app-store/).

 Of course, there is an alternative to a JIT recompiler, called an "interpreter", but this is many times slower than the JIT method. So while it would work, it would be unplayable. Either we'll have to wait until the iPhone 30 to get the interpreter running fast enough, or we have to hope that Apple loosens its restrictions a little.

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1938750/19272" target="_top" id="1938750">
  <img src="//a.impactradius-go.com/display-ad/19272-1938750" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1938750/19272" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://instagram-video-files.techidaily.com/new-in-2024-instagrams-backstage-pass-top-covert-strategies-revealed/"><u>[New] In 2024, Instagram’s Backstage Pass  Top Covert Strategies Revealed</u></a></li>
<li><a href="https://remote-screen-capture.techidaily.com/new-screencapture-2023-top-techs-recommendations-for-2024/"><u>[New] ScreenCapture 2023  Top Tech's Recommendations for 2024</u></a></li>
<li><a href="https://youtube-blog.techidaily.com/ed-2024-approved-unleashing-potential-the-art-of-youtube-seo-keywords/"><u>[Updated] 2024 Approved  Unleashing Potential  The Art of YouTube SEO Keywords</u></a></li>
<li><a href="https://article-tips.techidaily.com/updated-crafting-compelling-podcast-teasers/"><u>[Updated] Crafting Compelling Podcast Teasers</u></a></li>
<li><a href="https://extra-lessons.techidaily.com/2024-approved-5-exceptional-4k-gaming-screens/"><u>2024 Approved  5 Exceptional 4K Gaming Screens</u></a></li>
<li><a href="https://digital-screen-recording.techidaily.com/2024-approved-explore-the-safest-video-chat-apps-on-both-sides-of-the-market/"><u>2024 Approved  Explore the Safest Video Chat Apps on Both Sides of the Market</u></a></li>
<li><a href="https://buynow-help.techidaily.com/2024s-ultimate-selection-of-compact-and-portable-tv-screens-for-on-the-go-viewing-experience/"><u>2024'S Ultimate Selection of Compact and Portable TV Screens for On-the-Go Viewing Experience</u></a></li>
<li><a href="https://techtrends.techidaily.com/a-comprehensive-checklist-for-purchasing-a-tech-device-for-education-needs/"><u>A Comprehensive Checklist for Purchasing a Tech Device for Education Needs</u></a></li>
<li><a href="https://tech-recovery.techidaily.com/affordable-luxury-top-tier-tech-delights-to-try/"><u>Affordable Luxury: Top-Tier Tech Delights to Try</u></a></li>
<li><a href="https://buynow-help.techidaily.com/amazons-ultimate-prime-day-offers-for-202n-save-big-and-find-the-best-bargains/"><u>Amazon's Ultimate Prime Day Offers for 202N: Save Big and Find the Best Bargains!</u></a></li>
<li><a href="https://voice-adjusting.techidaily.com/audio-extraction-guide-for-updated-mkv-files-mkv-2023-edition/"><u>Audio Extraction Guide for Updated MKV Files (MKV-2023 Edition)</u></a></li>
<li><a href="https://buynow-help.techidaily.com/bringing-old-school-gaming-to-modern-apple-products-download-retroarch-for-iphone-ipad-and-apple-tv/"><u>Bringing Old-School Gaming to Modern Apple Products: Download RetroArch for iPhone, iPad & Apple TV!</u></a></li>
<li><a href="https://buynow-help.techidaily.com/discover-the-leading-free-virtual-private-network-vpn-options-for-optimal-online-privacy/"><u>Discover the Leading Free Virtual Private Network (VPN) Options for Optimal Online Privacy</u></a></li>
<li><a href="https://fox-cloud.techidaily.com/embracing-illusion-what-is-vrs-truth/"><u>Embracing Illusion  What Is VR's Truth?</u></a></li>
<li><a href="https://buynow-help.techidaily.com/experience-all-access-live-streaming-of-four-olympic-games-with-peacocks-unique-viewing-feature/"><u>Experience All-Access Live Streaming of Four Olympic Games with Peacock's Unique Viewing Feature</u></a></li>
<li><a href="https://buynow-help.techidaily.com/explore-elite-audio-quality-with-our-pick-of-leading-stereo-receivers-homes/"><u>Explore Elite Audio Quality with Our Pick of Leading Stereo Receivers Homes</u></a></li>
<li><a href="https://some-approaches.techidaily.com/free-access-or-upgrade-costs-can-you-download-the-newest-freemake-video-converter-at-no-charge/"><u>Free Access or Upgrade Costs? Can You Download the Newest Freemake Video Converter at No Charge?</u></a></li>
<li><a href="https://buynow-help.techidaily.com/get-more-bang-for-your-buck-with-these-7-tips-for-disneyplus-subscribers/"><u>Get More Bang for Your Buck with These 7 Tips for Disney+ Subscribers</u></a></li>
<li><a href="https://hardware-updates.techidaily.com/get-the-newest-updates-for-your-hp-deskjet-3700-driver-software-downloads-available-now/"><u>Get the Newest Updates for Your HP Deskjet 3700: Driver Software Downloads Available Now</u></a></li>
<li><a href="https://android-location.techidaily.com/getting-the-pokemon-go-gps-signal-not-found-11-error-in-zte-blade-a73-5g-drfone-by-drfone-virtual/"><u>Getting the Pokemon Go GPS Signal Not Found 11 Error in ZTE Blade A73 5G | Dr.fone</u></a></li>
<li><a href="https://android-location-track.techidaily.com/in-2024-how-to-track-vivo-y77t-location-without-installing-software-drfone-by-drfone-virtual-android/"><u>In 2024, How to Track Vivo Y77t Location without Installing Software? | Dr.fone</u></a></li>
<li><a href="https://screen-video-capture.techidaily.com/in-2024-streamlining-the-demo-process-in-adobe-captivate/"><u>In 2024, Streamlining the Demo Process in Adobe Captivate</u></a></li>
<li><a href="https://facebook-video-footage.techidaily.com/in-2024-youtubes-revenue-boost-new-500-subs-milestone/"><u>In 2024, YouTube's Revenue Boost  New 500 Subs Milestone</u></a></li>
<li><a href="https://extra-hints.techidaily.com/invaluable-list-of-prime-no-charge-sites-for-seamless-video-editing-experience/"><u>Invaluable List of Prime No-Charge Sites for Seamless Video Editing Experience</u></a></li>
<li><a href="https://win-forum.techidaily.com/navigating-the-worlds-leading-social-sites-youtube-instagram-facebook-and-twitter/"><u>Navigating the World's Leading Social Sites: YouTube, Instagram, Facebook & Twitter</u></a></li>
<li><a href="https://video-ai-editor.techidaily.com/new-switch-it-up-the-best-face-swap-apps-for-iphone-and-android-for-2024/"><u>New Switch It Up The Best Face Swap Apps for iPhone and Android for 2024</u></a></li>
<li><a href="https://extra-support.techidaily.com/next-gen-gaming-horizon-upcoming-bests-in-playstation-vr-for-2024/"><u>Next-Gen Gaming Horizon  Upcoming Bests in PlayStation VR for 2024</u></a></li>
<li><a href="https://snapchat-videos.techidaily.com/quick-start-methods-for-producing-and-perfecting-multiple-snaps-in-snapchat-for-2024/"><u>Quick Start Methods for Producing and Perfecting Multiple Snaps in Snapchat for 2024</u></a></li>
<li><a href="https://buynow-help.techidaily.com/read-reviews-from-trusted-tech-websites-and-communities-for-real-world-insights-on-build-stability-customer-support-warranty-offerings-and-upgrade-paths/"><u>Read Reviews From Trusted Tech Websites and Communities for Real-World Insights on Build Stability, Customer Support, Warranty Offerings, and Upgrade Paths.</u></a></li>
<li><a href="https://buynow-help.techidaily.com/rethinking-user-interfaces-why-touch-buttons-overload-is-harming-business/"><u>Rethinking User Interfaces: Why Touch Buttons Overload Is Harming Business</u></a></li>
<li><a href="https://techno-recovery.techidaily.com/step-by-step-switching-off-closed-captions-and-subtitles-in-amazons-prime-video-library/"><u>Step by Step: Switching Off Closed Captions and Subtitles in Amazon's Prime Video Library</u></a></li>
<li><a href="https://driver-download.techidaily.com/step-by-step-fixes-for-your-graphic-card-drivers-warning/"><u>Step-by-Step Fixes for Your Graphic Card Drivers Warning!</u></a></li>
<li><a href="https://win-howtos.techidaily.com/text-difficulty-windows-11-copy-issue/"><u>Text Difficulty: Windows 11 Copy Issue</u></a></li>
<li><a href="https://buynow-help.techidaily.com/the-letdown-of-ps2-on-ps5-master-the-art-of-gaming-with-pcsx2-instead/"><u>The Letdown of PS2 on PS5: Master the Art of Gaming with PCSX2 Instead!</u></a></li>
<li><a href="https://buynow-help.techidaily.com/the-revolutionary-raspberry-pi-pico-takes-on-dual-architectures-with-a-cutting-edge-risc-design/"><u>The Revolutionary Raspberry Pi Pico Takes on Dual Architectures with a Cutting-Edge RISC Design</u></a></li>
<li><a href="https://techidaily.com/the-way-to-recover-deleted-contacts-on-poco-m6-pro-4g-without-backup-by-fonelab-android-recover-contacts/"><u>The way to recover deleted contacts on Poco M6 Pro 4G without backup.</u></a></li>
<li><a href="https://buynow-help.techidaily.com/top-10-films-to-experience-in-stunning-clarity-on-your-latest-oled-television-set/"><u>Top 10 Films to Experience in Stunning Clarity on Your Latest OLED Television Set</u></a></li>
<li><a href="https://buynow-help.techidaily.com/top-5-longing-feelings-why-face-to-face-gaming-with-pals-beats-virtual-battles/"><u>Top 5 Longing Feelings: Why Face-to-Face Gaming with Pals Beats Virtual Battles</u></a></li>
<li><a href="https://buynow-help.techidaily.com/top-choice-couch-co-op-video-games-best-picks-for-enjoying-gaming-together/"><u>Top Choice Couch Co-Op Video Games: Best Picks for Enjoying Gaming Together</u></a></li>
<li><a href="https://buynow-help.techidaily.com/top-reason-elevate-your-pc-gaming-experience-with-a-controller-the-top-choice-for-gamers/"><u>Top Reason: Elevate Your PC Gaming Experience with a Controller - The Top Choice for Gamers!</u></a></li>
<li><a href="https://buynow-help.techidaily.com/top-rated-laptop-support-structures-a-comprehensive-review/"><u>Top-Rated Laptop Support Structures : A Comprehensive Review</u></a></li>
<li><a href="https://buynow-help.techidaily.com/top-rated-protective-covers-for-the-new-iphone-14-your-ultimate-guide/"><u>Top-Rated Protective Covers for the New iPhone 14: Your Ultimate Guide</u></a></li>
<li><a href="https://buynow-help.techidaily.com/ultimate-guide-to-choosing-the-perfect-protective-cases-for-ipads-9gen-in-2-023/"><u>Ultimate Guide to Choosing the Perfect Protective Cases for iPads (9Gen) in 2 023</u></a></li>
<li><a href="https://buynow-help.techidaily.com/uncover-the-true-intent-behind-apples-latest-strategy-on-game-emulation/"><u>Uncover the True Intent Behind Apple's Latest Strategy on Game Emulation</u></a></li>
<li><a href="https://buynow-help.techidaily.com/understanding-1440p-the-complete-guide-to-quad-hd-qhd-display/"><u>Understanding 1440P: The Complete Guide to Quad HD (QHD) Display</u></a></li>
<li><a href="https://extra-information.techidaily.com/unlock-creative-potential-editing-videos-via-windows-photos-and-story-remix/"><u>Unlock Creative Potential  Editing Videos via Windows Photos and Story Remix</u></a></li>
<li><a href="https://buynow-help.techidaily.com/unplugging-from-the-web-why-securing-or-turning-off-your-vizio-smart-tv-is-essential/"><u>Unplugging From the Web: Why Securing or Turning Off Your Vizio Smart TV Is Essential</u></a></li>
<li><a href="https://buynow-help.techidaily.com/update-on-google-tv-why-purchasing-tv-episodes-directly-from-the-platform-is-a-thing-of-the-past/"><u>Update on Google TV - Why Purchasing TV Episodes Directly From the Platform Is a Thing of the Past</u></a></li>
<li><a href="https://buynow-help.techidaily.com/upgrade-legacy-speakers-today-discover-wiims-latest-breakthrough-in-ultra-streaming-technology-for-enhanced-acoustics/"><u>Upgrade Legacy Speakers Today! Discover WiiM's Latest Breakthrough in Ultra Streaming Technology for Enhanced Acoustics.</u></a></li>
<li><a href="https://buynow-help.techidaily.com/upgrading-your-mobile-pc-with-microsofts-improved-windows-features/"><u>Upgrading Your Mobile PC with Microsoft's Improved Windows Features</u></a></li>
<li><a href="https://fake-location.techidaily.com/what-is-fake-gps-location-pro-and-is-it-good-on-xiaomi-redmi-note-13-proplus-5g-drfone-by-drfone-virtual-android/"><u>What is Fake GPS Location Pro and Is It Good On Xiaomi Redmi Note 13 Pro+ 5G? | Dr.fone</u></a></li>
<li><a href="https://buynow-help.techidaily.com/why-classic-game-consoles-trounce-smartphones-a-look-at-5-key-benefits-for-gamers/"><u>Why Classic Game Consoles Trounce Smartphones: A Look at 5 Key Benefits for Gamers</u></a></li>
<li><a href="https://buynow-help.techidaily.com/why-invest-in-online-radio-even-with-the-popularity-of-streaming-services/"><u>Why Invest in Online Radio Even with the Popularity of Streaming Services</u></a></li>
<li><a href="https://buynow-help.techidaily.com/why-leaving-spotify-is-harder-than-youd-think-even-if-you-hate-it/"><u>Why Leaving Spotify Is Harder Than You'd Think Even If You Hate It</u></a></li>
<li><a href="https://buynow-help.techidaily.com/why-mid-range-processors-suffice-in-todays-gaming-world/"><u>Why Mid-Range Processors Suffice in Today's Gaming World</u></a></li>
<li><a href="https://buynow-help.techidaily.com/why-the-lack-of-achievements-on-the-switch-could-be-a-positive-thing/"><u>Why the Lack of Achievements on The Switch Could Be a Positive Thing</u></a></li>
<li><a href="https://buynow-help.techidaily.com/why-vintage-game-systems-appear-poorly-on-contemporary-televisions-causes-and-solutions/"><u>Why Vintage Game Systems Appear Poorly on Contemporary Televisions: Causes & Solutions</u></a></li>
<li><a href="https://buynow-help.techidaily.com/youtube-music-launches-shareable-personalized-radio-feature/"><u>YouTube Music Launches Shareable Personalized Radio Feature</u></a></li>
</ul></div>
