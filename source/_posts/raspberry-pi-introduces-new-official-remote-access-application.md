---
title: Raspberry Pi Introduces New Official Remote Access Application
date: 2025-01-22T17:11:31.525Z
updated: 2025-01-29T16:55:56.176Z
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
<li><a href="https://fox-access.techidaily.com/new-in-2024-flight-finesse-crafting-the-top-10-endurance-drone-lineup/"><u>[New] In 2024, Flight Finesse Crafting the Top 10 Endurance Drone Lineup</u></a></li>
<li><a href="https://extra-lessons.techidaily.com/updated-breaking-down-augmented-realitys-mysteries/"><u>[Updated] Breaking Down Augmented Reality's Mysteries</u></a></li>
<li><a href="https://buynow-help.techidaily.com/best-voip-option-of-2023-is-vonage-no-longer-leading-the-pack/"><u>Best VoIP Option of 2023 - Is Vonage No Longer Leading the Pack?</u></a></li>
<li><a href="https://buynow-help.techidaily.com/exploring-the-benefits-of-the-fitbit-versa-2-a-complete-review-for-smartwatch-enthusiasts-seeking-fitness-solutions/"><u>Exploring the Benefits of the Fitbit Versa 2: A Complete Review for Smartwatch Enthusiasts Seeking Fitness Solutions</u></a></li>
<li><a href="https://win-amazing.techidaily.com/how-to-resolve-connectivity-issues-for-lg-hardware-via-usb-in-windows-operating-systems/"><u>How to Resolve Connectivity Issues for LG Hardware via USB in Windows Operating Systems</u></a></li>
<li><a href="https://tiktok-video-files.techidaily.com/seamless-tiktok-to-high-quality-mp4-format/"><u>Seamless TikTok to High-Quality MP4 Format</u></a></li>
<li><a href="https://buynow-help.techidaily.com/the-ultimate-guide-to-the-clearstream-eclipse-a-perfect-blend-of-power-and-practicality/"><u>The Ultimate Guide to the ClearStream Eclipse - A Perfect Blend of Power and Practicality</u></a></li>
<li><a href="https://screen-sharing-recording.techidaily.com/versatile-pci-support-tools-for-win-users/"><u>Versatile PCI Support Tools for Win Users</u></a></li>
<li><a href="https://buynow-help.techidaily.com/vtech-kidizoom-dual-cam-happiness/"><u>VTech Kidizoom Dual-Cam Happiness</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/_SbYznUy_zY?si=ThBkP934r3mizi48" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

