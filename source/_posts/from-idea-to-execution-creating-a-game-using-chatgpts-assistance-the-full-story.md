---
title: "From Idea to Execution: Creating a Game Using ChatGPT's Assistance – The Full Story"
date: 2024-09-04T16:15:10.053Z
updated: 2024-09-05T16:15:10.053Z
tags:
  - games
  - tv
  - movies
categories:
  - tech
thumbnail: https://thmb.techidaily.com/fc56be1104b47b174a9a13d9255575e8e01dfcc34ec60d7f7f9e3cbb3a84553c.jpg
---

## From Idea to Execution: Creating a Game Using ChatGPT's Assistance – The Full Story

### Key Takeaways

* Game engines understood by ChatGPT are suitable for coding game prototypes.
* Coding assistance from ChatGPT requires a decent understanding of the game engine being used.
* Expect ChatGPT to provide close, but not exact, solutions to coding problems. You still need to review and revise the code provided by ChatGPT.

 AI is the new buzzword that everyone seems to be talking about. Even phones are getting fully implemented AI applications, but there's a lot more you could do with tools like ChatGPT, including coding a game. I've been developing games for almost a decade, and have even released a few projects and participated in a couple of [game jams on Itch](https://itch.io/jams).

 When I discovered ChatGPT, the first thing I wanted to do was see if I could use it in game development. As always, ChatGPT is eager to help and almost feels like the world's most into-it intern.

##  Can ChatGPT Code a Game for You?

![ChatGPT gives me a list of ideas that I could potentially make into a game](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/screenshot-1.png) 

 It's quickly apparent that GPT's willingness to [teach you to code](https://fox-helps.techidaily.com/navigating-gif-storage-and-use-in-the-digital-age-iphone/) a game is well-meaning but requires you to understand a bit about what you're doing. As someone who's been an amateur game developer for more than a decade, I know a little bit about coding a game. In using GPT to help me, I was interested in seeing how sophisticated it was for producing a playable game prototype.

###  It Certainly Understands Game Engines

 A game engine is what a developer uses to create a game. Several game engines are available, including [Unreal Engine](https://www.unrealengine.com/en-US), [Godot](https://godotengine.org/), and [Unity](https://unity.com/). As someone who knows Unity well, I decided to use this as my development engine. I asked a few general questions (that I know the answer to) to ensure that [ChatGPT wouldn't start hallucinating](https://audio-shaping.techidaily.com/strategies-for-minimizing-large-scale-video-and-audio-data/) about my game engine.

![ChatGPT describes the steps in building a player character](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/chatgpt-seems-to-know-some-stuff-1.png) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2030395/7443" target="_top" id="2030395">
  <img src="//a.impactradius-go.com/display-ad/7443-2030395" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2030395/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 After sorting out that it at least knew what it was doing, I decided to give the framework for my project, which included:

* Random generation of a scrolling background
* Having a player character controlled by directional buttons, with mouse buttons for firing
* A point system with a leaderboard
* An endless amount of enemies, so players can play casually

 ChatGPT was very helpful in offering code solutions for some of the things I would need to create this game. For example, I asked it for some code for a projectile I would fire from the player's position when they hit the "Fire" button, and it gave me this:

        `using UnityEngine;  
  
public class Projectile : MonoBehaviour  

    public float speed = 10f; // Adjust this value to control projectile speed  
  
    void Start()  

        // Move the projectile forward in its local space (assuming it's facing right)  
        GetComponent<Rigidbody2D>().velocity = transform.right * speed;  

  
    void OnTriggerEnter2D(Collider2D other)  

        // Check if the projectile collides with an enemy or other objects  
        if (other.CompareTag("Enemy"))  

            // Handle enemy damage or destruction  
            Destroy(other.gameObject); // Destroy the enemy  
            Destroy(gameObject); // Destroy the projectile  

        else if (other.CompareTag("Wall"))  

            // Destroy the projectile if it collides with a wall  
            Destroy(gameObject);  


}`
    
 Notably, it gave me well-commented code so I could follow along as a beginner programmer. Many places suggest that you could [learn to code using AI](https://learntocodewith.me/resources/ai-coding/), and the inclusion of well-commented code is part of that. You won't have to worry if there are errors in your code if you can trace them comment by comment. However, when using GPT to build a game, I encountered several issues that would defeat a newcomer to game development.

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
###  ChatGPT Is Far From Perfect

 LLMs are only as good (or as bad) as the prompts the user gives them. For example, a user could easily [generate anime-type characters with MidJourney](https://some-tips.techidaily.com/new-ultimate-strategies-pinterest-to-mp3-migration-guide/) by including a few words to clarify the prompt's end result. However, when building a game with ChatGPT, I found that there were times when the engine simply didn't pick up what I was putting down.

![An error happens that I can't seem to figure out, so I ask GPT for help](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/a-wild-unexpected-behavior-appears.png) 

<!-- affiliate ads begin -->
<span id="1531879">
					<video width="864" height="1536" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1531879.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/16446-1531879">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1531879.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:540px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Flaganoo.pxf.io%2Fc%2F5597632%2F1531879%2F16446'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1531879/16446" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 In this example, I encountered an issue with spawning my projectiles, with all the "bullets" being deflected when the player moves. While this could create some interesting play patterns, I decided to ask it to fix the problem, and it suggested a fix. Unfortunately, the fix didn't work.

![GPT's responses doesn't fix the error I keep having](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/the-error-is-still-there.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1997662/19272" target="_top" id="1997662">
  <img src="//a.impactradius-go.com/display-ad/19272-1997662" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1997662/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 I eventually fixed it myself, but it highlighted a major issue with using ChatGPT to code a game: there are some things it doesn't know.

![A Do-it-Yourself Fix For The Programming Problem](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/diy-fix.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2036472/19272" target="_top" id="2036472">
  <img src="//a.impactradius-go.com/display-ad/19272-2036472" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2036472/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 I eventually put together the game using a few suggestions from GPT about the persistent score as well as the random generation algorithm and scrolling for the game background. You can [play the final game here](https://zandoliearts.itch.io/the-unfriendly-skies).

##  Does It Work With Other Game Engines?

 I know ChatGPT was very good with Unity once I could sort out some of the issues I ran into above. However, I wondered how coding a game with ChatGPT would work for a less-popular engine like Godot. I'm not exactly an expert in Godot, having used it far less than I did Unity. I decided to ask ChatGPT a few questions:

![GPT gives me a piece of code that is outdated because of GPT's limitations](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/gpt-s-godot-problem-1.png) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2049370/7443" target="_top" id="2049370">
  <img src="//a.impactradius-go.com/display-ad/7443-2049370" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2049370/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
GPT's Godot Problem

 For those who use Godot regularly, the issue is immediately obvious. ChatGPT stopped learning in 2021 or thereabouts (at least for the free version). The script GPT gave me was based on its knowledge of Godot 2.x, which is a heavily outdated version of the current 4.x version. The glaring problem is the use of KinematicBody2D, which was replaced by CharacterBody2D in later iterations of the language.

##  How Much Skill Do You Need to Code a Game With ChatGPT?

 If you're considering making the next Legend of Zelda: Breath of the Wild using ChatGPT, you should probably temper your expectations. You need to have a decent understanding of the engine you're working in to use ChatGPT as a coding assistant.

 Other assistants like Microsoft Copilot might be better with general code and could help to a greater degree. The big issue is that these LLMs are looking at an abstract problem, and they're seeing it without actually seeing it.

 In simpler language, you know what the game you're making should look like and how things in it should behave. You can explain it to ChatGPT what you want, and it will give you something close to (but not quite) what your game needs. To make it behave the way you want it to, you'll have to fiddle around with the code that GPT gives you.

##  Should You Code a Game With ChatGPT?

![Screenshot of My Game's Title Page](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/screen-1-1.jpg) 

 Game development is a complex field, but thanks to engines like those mentioned above, it is much more approachable for the general public. A skilled developer could spend a few hours putting together a game that works and has all the things they want in it.

 This particular project took me a total of 48 hours from start to finish. The more complex the game, the more time and effort it will take. That's not counting the amount of time you'd have to throw into asset sourcing and development. It could get to be a pretty large project.

 If you do decide to code a game with ChatGPT assisting, here are a few things to keep in mind:

* ChatGPT can make mistakes in code.
* ChatGPT might give you outdated code, requiring you to spend hours googling for a fix.
* AI can't make game assets as of yet (not good 2D assets, anyway) so you'll have to source assets separately.
* Some of the suggestions ChatGPT gives you won't work and might lead you to a dead end, requiring you to rethink your implementation.

---

 If anyone asked me today if they could learn to code a game with ChatGPT from scratch without any knowledge of the engine, I'd have to tell them no.

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
<li><a href="https://instagram-videos.techidaily.com/new-2024-approved-saving-your-best-on-instagram-a-comprehensive-guide/"><u>[New] 2024 Approved  Saving Your Best on Instagram  A Comprehensive Guide</u></a></li>
<li><a href="https://digital-screen-recording.techidaily.com/new-chilly-cinematography-comprehensive-ice-cream-monitoring-tutorial-for-2024/"><u>[New] Chilly Cinematography  Comprehensive Ice Cream Monitoring Tutorial for 2024</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/new-expertly-record-your-browser-adventures-with-top-5-capturers-for-2024/"><u>[New] Expertly Record Your Browser Adventures with Top 5 Capturers for 2024</u></a></li>
<li><a href="https://instagram-video-files.techidaily.com/new-instantaneous-instagram-video-experience-for-2024/"><u>[New] Instantaneous Instagram Video Experience for 2024</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/updated-instant-viral-potential-learn-kinemaster-memes/"><u>[Updated] Instant Viral Potential  Learn KineMaster Memes</u></a></li>
<li><a href="https://video-screen-grab.techidaily.com/updated-techniques-for-efficient-zoom-meeting-recordings/"><u>[Updated] Techniques for Efficient Zoom Meeting Recordings</u></a></li>
<li><a href="https://buynow-info.techidaily.com/affordable-ssl-vendors-a-comprehensible-guide/"><u>Affordable SSL Vendors: A Comprehensible Guide</u></a></li>
<li><a href="https://buynow-help.techidaily.com/comparing-ipad-pro-and-surface-pro-key-distinctions-revealed/"><u>Comparing IPad Pro and Surface Pro: Key Distinctions Revealed</u></a></li>
<li><a href="https://buynow-help.techidaily.com/efficient-heat-dissipation-with-a-cheap-laptop-tray-the-topmate-c302-breakdown/"><u>Efficient Heat Dissipation with a Cheap Laptop Tray: The TopMate C302 Breakdown</u></a></li>
<li><a href="https://buynow-help.techidaily.com/elevate-your-blogging-income-with-buysellads-monetization-tactics/"><u>Elevate Your Blogging Income with BuySellAds Monetization Tactics</u></a></li>
<li><a href="https://buynow-help.techidaily.com/enhancing-wifi-coverage-a-professional-review-on-the-performance-of-the-tp-link-re505x-extender/"><u>Enhancing WiFi Coverage: A Professional Review on the Performance of the TP-Link RE505X Extender</u></a></li>
<li><a href="https://buynow-help.techidaily.com/expert-analysis-why-the-samsung-qn55q6f-is-a-top-contender-in-4k-hdr-smart-tvs/"><u>Expert Analysis: Why the Samsung QN55Q6F Is a Top Contender in 4K HDR Smart TVs</u></a></li>
<li><a href="https://buynow-help.techidaily.com/exploring-nvidia-shield-tv-pros-features-the-perfect-gaming-media-player/"><u>Exploring Nvidia Shield TV Pro's Features: The Perfect Gaming Media Player</u></a></li>
<li><a href="https://buynow-help.techidaily.com/exploring-the-best-features-of-the-stylish-and-smart-withings-move-watch/"><u>Exploring the Best Features of the Stylish and Smart Withings Move Watch</u></a></li>
<li><a href="https://buynow-help.techidaily.com/fitbit-versa-smartwatch-examined-cost-effective-style-for-health-enthusiasts/"><u>Fitbit Versa Smartwatch Examined: Cost-Effective Style for Health Enthusiasts</u></a></li>
<li><a href="https://buynow-help.techidaily.com/gamers-delight-the-premier-console-selection-for-an-epic-year/"><u>Gamers' Delight: The Premier Console Selection for an Epic Year</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/guide-to-mirror-your-infinix-hot-40-to-other-android-devices-drfone-by-drfone-android/"><u>Guide to Mirror Your Infinix Hot 40 to Other Android devices | Dr.fone</u></a></li>
<li><a href="https://buynow-help.techidaily.com/immerse-yourself-in-the-thrill-a-detailed-evaluation-of-nhl-19s-interactive-online-experience/"><u>Immerse Yourself in the Thrill – A Detailed Evaluation of NHL 19’S Interactive Online Experience</u></a></li>
<li><a href="https://pokemon-go-android.techidaily.com/in-2024-here-are-some-reliable-ways-to-get-pokemon-go-friend-codes-for-honor-x50iplus-drfone-by-drfone-virtual-android/"><u>In 2024, Here Are Some Reliable Ways to Get Pokemon Go Friend Codes For Honor X50i+ | Dr.fone</u></a></li>
<li><a href="https://android-transfer.techidaily.com/in-2024-how-can-you-transfer-files-from-vivo-v30-pro-to-iphone-151413-drfone-by-drfone-transfer-from-android-transfer-from-android/"><u>In 2024, How Can You Transfer Files From Vivo V30 Pro To iPhone 15/14/13? | Dr.fone</u></a></li>
<li><a href="https://sim-unlock.techidaily.com/in-2024-sim-unlock-oneplus-open-phones-without-code-2-ways-to-remove-android-sim-lock-by-drfone-android/"><u>In 2024, Sim Unlock OnePlus Open Phones without Code 2 Ways to Remove Android Sim Lock</u></a></li>
<li><a href="https://buynow-help.techidaily.com/kobo-nia-review-how-this-e-reader-holds-its-own-against-amazons-best/"><u>Kobo Nia Review: How This E-Reader Holds Its Own Against Amazon's Best</u></a></li>
<li><a href="https://buynow-help.techidaily.com/maximizing-music-at-parties-a-comprehensive-review-of-the-ion-audio-tailgater-plus/"><u>Maximizing Music at Parties: A Comprehensive Review of the ION Audio Tailgater Plus</u></a></li>
<li><a href="https://buynow-help.techidaily.com/score-big-with-limited-time-deals-on-premium-samsung-tech-gadgets/"><u>Score Big with Limited-Time Deals on Premium Samsung Tech Gadgets</u></a></li>
<li><a href="https://sound-issues.techidaily.com/solving-the-problem-of-an-inoperative-headset-microphone/"><u>Solving the Problem of an Inoperative Headset Microphone</u></a></li>
<li><a href="https://buynow-help.techidaily.com/the-best-pastime-games-to-enjoy-during-down-time/"><u>The Best Pastime Games to Enjoy During Down Time</u></a></li>
<li><a href="https://fox-glue.techidaily.com/the-essential-guide-to-metaverse-brand-strategies-for-2024/"><u>The Essential Guide to Metaverse Brand Strategies for 2024</u></a></li>
<li><a href="https://buynow-help.techidaily.com/top-of-the-pup-pack-an-extensive-evaluation-of-the-best-dog-camera-on-the-market-furbo/"><u>Top of the Pup Pack: An Extensive Evaluation of The Best Dog Camera on the Market – Furbo</u></a></li>
<li><a href="https://buynow-help.techidaily.com/ultimate-guide-to-the-lenovo-thinkpad-x1-titanium-yoga-the-ideal-choice-for-fanatical-thinkpad-lovers/"><u>Ultimate Guide to the Lenovo ThinkPad X1 Titanium Yoga - The Ideal Choice for Fanatical ThinkPad Lovers</u></a></li>
<li><a href="https://buynow-help.techidaily.com/unleashing-the-potential-of-the-portable-beast-in-depth-look-at-apples-ipad-mini-5/"><u>Unleashing the Potential of the Portable Beast - In Depth Look at Apple's iPad Mini 5</u></a></li>
<li><a href="https://buynow-help.techidaily.com/unveiling-parental-supervision-and-long-range-expertise-with-the-powerful-synology-rt2600ac-wireless-networking-appliance/"><u>Unveiling Parental Supervision and Long-Range Expertise with the Powerful Synology RT2600ac Wireless Networking Appliance</u></a></li>
<li><a href="https://driver-install.techidaily.com/update-for-improved-connectivity-hdmi-on-windows-10-11/"><u>Update for Improved Connectivity: HDMI on Windows 10, 11</u></a></li>
<li><a href="https://buynow-help.techidaily.com/xbox-series-s-evaluation-astonishing-tech-in-compact-design/"><u>Xbox Series S Evaluation: Astonishing Tech in Compact Design</u></a></li>
</ul></div>
