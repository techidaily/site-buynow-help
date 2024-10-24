---
title: Raspberry Pi Introduces New Official Remote Access Application
date: 2024-10-21T05:17:19.023Z
updated: 2024-10-24T08:15:17.361Z
tags:
  - games
  - tv
  - movies
categories:
  - tech
thumbnail: https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/8-1.png
---

## Raspberry Pi Introduces New Official Remote Access Application

Now available in beta, Raspberry Pi Connect provides remote access to your Pi desktop from a web browser. Install the Pi Connect beta, sign in with a Raspberry Pi ID, and you're good to go.

 This is the first _official_ remote access client for Raspberry Pi. Yes, you could already establish a remote connection over [VNC](https://www.raspberrypi.com/documentation/computers/remote-access.html#vnc), but VNC is mainly for technical support and can be difficult to set up. Third-party remote access tools, while robust, may fail to keep up with major Pi OS upgrades or under-the-hood OS changes. For example, the latest Pi OS Bookworm release completely ended X remote desktop support by switching to the newer Wayland technology.

[Raspberry Pi Connect](https://www.raspberrypi.com/software/connect/) is easy to install but requires a 64-bit version of [Pi OS Bookworm](https://some-tips.techidaily.com/2024-approved-the-experts-list-of-top-vector-stock-portals/) with Wayland window server. So, hardware-wise, you're limited to the Pi 5, Pi 4, and Pi 400\. If you own an eligible Raspberry Pi but need to upgrade to OS Bookworm, go visit the [Raspberry Pi Imager](https://www.raspberrypi.com/software/).

 Once you're running Pi OS Bookworm, open a terminal window and enter the following:

sudo apt update

    
                    sudo apt upgrade

    
                    sudo apt install rpi-connect

 Reboot your Raspberry Pi and click the Connect icon (spinning wheel) icon at the right side of your menu bar. You'll be asked to sign in with a Raspberry Pi ID. Finally, you can access your Raspberry Pi from any computer by visiting the [Connect Portal](https://connect.raspberrypi.com/sign-in). It should work for both local and remote Raspberry Pi computers.

 Raspberry Pi Connect automatically turns on at startup. If you need to pause or disable this service, click the Connect icon in your Raspberry Pi's menu bar and select "Disable screen sharing" or "Sign out." If you plan on sharing Connect with other users, or if you're deeply concerned about security, I suggest enabling [enhanced logging](https://www.raspberrypi.com/documentation/services/connect.html#enable-enhanced-logging) for the service.

 As a beta app, Pi Connect may be a bit buggy. It also lacks the ability to share multiple screens at a time, so if your Pi computer is connected to multiple monitors, you may run into some weird problems. Also, if the Connect service needs to relay your traffic, you'll experience a lot of lag. The Pi Foundation currently has just one TURN relay server in the UK and doesn't know how often relaying will be required.

 For additional information and instructions, check out the [Raspberry Pi Connect documentation](https://www.raspberrypi.com/documentation/services/connect.html). The Connect service will be free forever, but traffic relays may cost money at some point, depending on how things work out.

 Source: [The Raspberry Pi Foundation](https://www.raspberrypi.com/news/raspberry-pi-connect/)

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
<li><a href="https://instagram-clips.techidaily.com/new-in-2024-10-best-tags-analyzing-apps-fb-twt-and-ig-platforms/"><u>[New] In 2024, 10 Best Tags Analyzing Apps FB, Twt & IG Platforms</u></a></li>
<li><a href="https://extra-approaches.techidaily.com/new-revolutionize-your-visual-experience-top-10-4k-mac-displays/"><u>[New] Revolutionize Your Visual Experience - Top 10 4K Mac Displays</u></a></li>
<li><a href="https://fox-links.techidaily.com/2024-approved-from-basics-to-bonus-elevate-your-cam-game/"><u>2024 Approved From Basics to Bonus Elevate Your Cam Game</u></a></li>
<li><a href="https://buynow-help.techidaily.com/2024s-most-outstanding-television-models-reviewed-find-the-perfect-set-for-you/"><u>2024'S Most Outstanding Television Models Reviewed: Find the Perfect Set for You</u></a></li>
<li><a href="https://buynow-help.techidaily.com/a-comprehensive-guide-to-the-most-advanced-sprinkler-automation-solutions/"><u>A Comprehensive Guide to the Most Advanced Sprinkler Automation Solutions</u></a></li>
<li><a href="https://buynow-help.techidaily.com/affordable-and-powerful-laptop-picks-for-the-savvy-shopper-2023-edition/"><u>Affordable & Powerful Laptop Picks for the Savvy Shopper - 2023 Edition</u></a></li>
<li><a href="https://buynow-help.techidaily.com/affordable-and-high-performance-mechanical-keyboards-below-50-price-tag/"><u>Affordable and High-Performance Mechanical Keyboards Below $50 Price Tag</u></a></li>
<li><a href="https://android-frp.techidaily.com/in-2024-a-quick-guide-to-oppo-find-x7-frp-bypass-instantly-by-drfone-android/"><u>In 2024, A Quick Guide to Oppo Find X7 FRP Bypass Instantly</u></a></li>
<li><a href="https://youtube-web.techidaily.com/24-simplified-guide-instant-deletion-methods-for-youtube-discussions/"><u>In 2024, Simplified Guide Instant Deletion Methods for Youtube Discussions</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<span id="1936838">
					<video width="374" height="48" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1936838.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/18409-1936838">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1936838.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:234px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fcoinrule.sjv.io%2Fc%2F5597632%2F1936838%2F18409'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1936838/18409" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

