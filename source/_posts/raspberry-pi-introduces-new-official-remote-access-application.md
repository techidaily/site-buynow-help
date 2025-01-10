---
title: Raspberry Pi Introduces New Official Remote Access Application
date: 2025-01-02T23:19:55.360Z
updated: 2025-01-09T21:15:44.422Z
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
<li><a href="https://facebook-video-share.techidaily.com/new-cutting-edge-free-and-easy-top-11-youtube-title-inventors-for-2024/"><u>[New] Cutting-Edge, Free, and Easy Top 11 YouTube Title Inventors for 2024</u></a></li>
<li><a href="https://extra-approaches.techidaily.com/2024-approved-quick-steps-for-adding-speech-to-text-in-powerpoint-slides/"><u>2024 Approved Quick Steps for Adding Speech-to-Text in PowerPoint Slides</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/2024-approved-top-8-photo-grid-online-makers-to-polish-your-pictures/"><u>2024 Approved Top 8 Photo Grid Online Makers to Polish Your Pictures</u></a></li>
<li><a href="https://buynow-reviews.techidaily.com/comprehensive-samsung-cf591-assessment-top-choice-for-gamers/"><u>Comprehensive Samsung CF591 Assessment: Top Choice for Gamers</u></a></li>
<li><a href="https://tech-renaissance.techidaily.com/critical-bugs-in-macos-sierra-version-144-exposed-prepare-before-upgrading-insights-from-zdnet/"><u>Critical Bugs in macOS Sierra Version 14.4 Exposed - Prepare Before Upgrading: Insights From ZDNet</u></a></li>
<li><a href="https://unlock-android.techidaily.com/top-12-prominent-xiaomi-redmi-note-12-5g-fingerprint-not-working-solutions-by-drfone-android/"><u>Top 12 Prominent Xiaomi Redmi Note 12 5G Fingerprint Not Working Solutions</u></a></li>
<li><a href="https://buynow-help.techidaily.com/uncovering-the-capabilities-of-the-orbi-whole-home-wi-fi-system-a-detailed-review-on-performance-and-reliability/"><u>Uncovering the Capabilities of the Orbi Whole Home Wi-Fi System - A Detailed Review on Performance and Reliability</u></a></li>
<li><a href="https://buynow-help.techidaily.com/unlock-local-treasures-browse-free-classified-options-on-oodle-now/"><u>Unlock Local Treasures: Browse Free Classified Options on Oodle Now</u></a></li>
<li><a href="https://buynow-help.techidaily.com/unveiling-portability-meets-performance-the-msi-pro-mp161e2-display-review/"><u>Unveiling Portability Meets Performance: The MSI Pro MP161E2 Display Review</u></a></li>
<li><a href="https://buynow-help.techidaily.com/unveiling-the-features-and-performance-of-garmin-forerunner-265/"><u>Unveiling The Features and Performance of Garmin Forerunner 265</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-the-leading-laptops-of-2eplus24-a-comprehensive-review-by-apple-dell-and-competitors-zdnets-analysis/"><u>Unveiling the Leading Laptops of 2E+24: A Comprehensive Review by Apple, Dell & Competitors - ZDNet's Analysis</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/8U3ooyFiAB4?si=yXPQrDhMBEJwN2EZ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

