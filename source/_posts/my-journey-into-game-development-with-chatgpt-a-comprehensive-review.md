---
title: "My Journey Into Game Development with ChatGPT: A Comprehensive Review"
date: 2024-09-04T16:15:11.154Z
updated: 2024-09-05T16:15:11.154Z
tags:
  - games
  - tv
  - movies
categories:
  - tech
thumbnail: https://thmb.techidaily.com/34062c0c76761441d1daaab882479cf039a7dd266a5c393fca1f08310200c903.jpg
---

## My Journey Into Game Development with ChatGPT: A Comprehensive Review

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
<a href="https://imp.i357552.net/c/5597632/1006793/11832" target="_top" id="1006793">
  <img src="//a.impactradius-go.com/display-ad/11832-1006793" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://imp.i357552.net/i/5597632/1006793/11832" style="position:absolute;visibility:hidden;" border="0" />
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

###  ChatGPT Is Far From Perfect

 LLMs are only as good (or as bad) as the prompts the user gives them. For example, a user could easily [generate anime-type characters with MidJourney](https://some-tips.techidaily.com/new-ultimate-strategies-pinterest-to-mp3-migration-guide/) by including a few words to clarify the prompt's end result. However, when building a game with ChatGPT, I found that there were times when the engine simply didn't pick up what I was putting down.

![An error happens that I can't seem to figure out, so I ask GPT for help](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/a-wild-unexpected-behavior-appears.png) 

 In this example, I encountered an issue with spawning my projectiles, with all the "bullets" being deflected when the player moves. While this could create some interesting play patterns, I decided to ask it to fix the problem, and it suggested a fix. Unfortunately, the fix didn't work.

![GPT's responses doesn't fix the error I keep having](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/the-error-is-still-there.png) 

<!-- affiliate ads begin -->
<span id="1975555">
					<video width="128" height="480" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1975555.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/22993-1975555">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1975555.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:80px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fhomestyler.sjv.io%2Fc%2F5597632%2F1975555%2F22993'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1975555/22993" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 I eventually fixed it myself, but it highlighted a major issue with using ChatGPT to code a game: there are some things it doesn't know.

![A Do-it-Yourself Fix For The Programming Problem](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/diy-fix.png) 

 I eventually put together the game using a few suggestions from GPT about the persistent score as well as the random generation algorithm and scrolling for the game background. You can [play the final game here](https://zandoliearts.itch.io/the-unfriendly-skies).

<!-- affiliate ads begin -->
<span id="1983549">
					<video width="576" height="240" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1983549.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/22993-1983549">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1983549.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:360px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fhomestyler.sjv.io%2Fc%2F5597632%2F1983549%2F22993'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1983549/22993" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
##  Does It Work With Other Game Engines?

 I know ChatGPT was very good with Unity once I could sort out some of the issues I ran into above. However, I wondered how coding a game with ChatGPT would work for a less-popular engine like Godot. I'm not exactly an expert in Godot, having used it far less than I did Unity. I decided to ask ChatGPT a few questions:

![GPT gives me a piece of code that is outdated because of GPT's limitations](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/gpt-s-godot-problem-1.png) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2044586/7443" target="_top" id="2044586">
  <img src="//a.impactradius-go.com/display-ad/7443-2044586" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2044586/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
GPT's Godot Problem

 For those who use Godot regularly, the issue is immediately obvious. ChatGPT stopped learning in 2021 or thereabouts (at least for the free version). The script GPT gave me was based on its knowledge of Godot 2.x, which is a heavily outdated version of the current 4.x version. The glaring problem is the use of KinematicBody2D, which was replaced by CharacterBody2D in later iterations of the language.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2031472/7443" target="_top" id="2031472">
  <img src="//a.impactradius-go.com/display-ad/7443-2031472" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2031472/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
##  How Much Skill Do You Need to Code a Game With ChatGPT?

 If you're considering making the next Legend of Zelda: Breath of the Wild using ChatGPT, you should probably temper your expectations. You need to have a decent understanding of the engine you're working in to use ChatGPT as a coding assistant.

 Other assistants like Microsoft Copilot might be better with general code and could help to a greater degree. The big issue is that these LLMs are looking at an abstract problem, and they're seeing it without actually seeing it.

 In simpler language, you know what the game you're making should look like and how things in it should behave. You can explain it to ChatGPT what you want, and it will give you something close to (but not quite) what your game needs. To make it behave the way you want it to, you'll have to fiddle around with the code that GPT gives you.

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1938721/19272" target="_top" id="1938721">
  <img src="//a.impactradius-go.com/display-ad/19272-1938721" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1938721/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
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
<li><a href="https://twitter-clips.techidaily.com/updated-2024-approved-twitters-favorites-top-10-tiktok-vids/"><u>[Updated] 2024 Approved  Twitter's Favorites  Top 10 TikTok Vids</u></a></li>
<li><a href="https://fox-cloud.techidaily.com/updated-in-2024-top-strategies-for-finding-and-using-a-lost-iphone-x/"><u>[Updated] In 2024, Top Strategies for Finding & Using a Lost iPhone X</u></a></li>
<li><a href="https://facebook-record-videos.techidaily.com/updated-streamlining-long-videos-on-youtube-through-effective-chapter-management/"><u>[Updated] Streamlining Long Videos on YouTube Through Effective Chapter Management</u></a></li>
<li><a href="https://snapchat-videos.techidaily.com/updated-unleashing-your-creativity-advanced-techniques-for-boomers-for-2024/"><u>[Updated] Unleashing Your Creativity  Advanced Techniques for Boomers for 2024</u></a></li>
<li><a href="https://howto.techidaily.com/7-solutions-to-fix-chrome-crashes-or-wont-open-on-realme-c53-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>7 Solutions to Fix Chrome Crashes or Wont Open on Realme C53 | Dr.fone</u></a></li>
<li><a href="https://buynow-help.techidaily.com/affordable-masterpiece-monoprice-graphic-tablet-unveiled-quality-meets-economy/"><u>Affordable Masterpiece: Monoprice Graphic Tablet Unveiled - Quality Meets Economy</u></a></li>
<li><a href="https://buynow-help.techidaily.com/affordable-performance-powerhouse-the-elph-190-review/"><u>Affordable Performance Powerhouse: The ELPH 190 Review</u></a></li>
<li><a href="https://buynow-help.techidaily.com/amplifi-hd-smart-mesh-wi-fi-system-review-bid-farewell-to-wi-fi-signal-blackouts/"><u>Amplifi HD Smart Mesh Wi-Fi System Review: Bid Farewell to Wi-Fi Signal Blackouts</u></a></li>
<li><a href="https://buynow-help.techidaily.com/choosing-between-giants-a-comprehensive-guide-to-outlook-and-gmail-features/"><u>Choosing Between Giants: A Comprehensive Guide to Outlook & Gmail Features</u></a></li>
<li><a href="https://buynow-help.techidaily.com/costly-convenience-with-airpods-max-investment/"><u>Costly Convenience with AirPods Max Investment</u></a></li>
<li><a href="https://buynow-help.techidaily.com/epb-shield-tunnelling-is-designed-for-soft-ground-conditions-with-high-water-content-and-uses-a-balancing-mechanism-at-the-face-of-the-tunnel-to-maintain-st137/"><u>EPB Shield Tunnelling Is Designed for Soft Ground Conditions with High Water Content and Uses a Balancing Mechanism at the Face of the Tunnel to Maintain Stability.</u></a></li>
<li><a href="https://buynow-help.techidaily.com/examining-the-sony-xperia-5-portable-powerful-and-pricier-than-ever-before/"><u>Examining the Sony Xperia 5: Portable, Powerful, And Pricier Than Ever Before</u></a></li>
<li><a href="https://buynow-help.techidaily.com/experience-next-gen-television-with-the-sony-xbr4-groovy-x900f-a-4k-uhd-marvel-on-a-49-screen/"><u>Experience Next-Gen Television with the Sony XBR4 Groovy X900F - A 4K UHD Marvel on a 49 Screen</u></a></li>
<li><a href="https://buynow-help.techidaily.com/expert-analysis-of-the-samsung-gear-s3-frontier-an-expansive-smartwatch-with-cutting-edge-capabilities/"><u>Expert Analysis of the Samsung Gear S3 Frontier: An Expansive Smartwatch with Cutting-Edge Capabilities</u></a></li>
<li><a href="https://iphone-unlock.techidaily.com/in-2024-how-to-unlock-a-found-iphone-6s-plus-drfone-by-drfone-ios/"><u>In 2024, How To Unlock A Found iPhone 6s Plus? | Dr.fone</u></a></li>
<li><a href="https://buynow-help.techidaily.com/in-depth-analysis-of-the-highly-capable-dell-xps-13-convertible-notebook/"><u>In-Depth Analysis of the Highly Capable Dell XPS 13 Convertible Notebook</u></a></li>
<li><a href="https://buynow-help.techidaily.com/in-depth-review-unveiling-the-charms-and-drawbacks-of-the-premium-priced-google-pixelbook-go/"><u>In-Depth Review: Unveiling the Charms and Drawbacks of the Premium-Priced Google Pixelbook Go</u></a></li>
<li><a href="https://buynow-help.techidaily.com/inside-look-at-the-fastest-device-for-streaming-the-ultimate-amazon-fire-tv-cube-review/"><u>Inside Look at The Fastest Device for Streaming – The Ultimate Amazon Fire TV Cube Review</u></a></li>
<li><a href="https://buynow-help.techidaily.com/mlb-the-show-19-analysis-when-baseball-meets-strategic-role-playing-adventures/"><u>MLB The Show 19 Analysis: When Baseball Meets Strategic Role-Playing Adventures</u></a></li>
<li><a href="https://buynow-help.techidaily.com/navigating-the-best-netgear-wifi-router-choices-for-enhanced-home-networking/"><u>Navigating the Best Netgear WiFi Router Choices for Enhanced Home Networking</u></a></li>
<li><a href="https://buynow-marvelous.techidaily.com/navigating-the-best-senior-friendly-mobile-tariffs/"><u>Navigating the Best Senior-Friendly Mobile Tariffs</u></a></li>
<li><a href="https://buynow-help.techidaily.com/paww-wavesound-3-review/"><u>Paww Wavesound 3 Review</u></a></li>
<li><a href="https://review-topics.techidaily.com/possible-solutions-to-restore-deleted-videos-from-red-magic-9-pro-by-fonelab-android-recover-video/"><u>Possible solutions to restore deleted videos from Red Magic 9 Pro</u></a></li>
<li><a href="https://buynow-help.techidaily.com/premium-picture-quality-at-a-bargain-the-inside-scoop-on-1byones-digital-amplified-indoor-hdtv-antenna/"><u>Premium Picture Quality at a Bargain: The Inside Scoop on 1Byone's Digital Amplified Indoor HDTV Antenna</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/recommended-best-applications-for-mirroring-your-vivo-y77t-screen-drfone-by-drfone-android/"><u>Recommended Best Applications for Mirroring Your Vivo Y77t Screen | Dr.fone</u></a></li>
<li><a href="https://iphone-unlock.techidaily.com/remove-device-supervision-from-your-apple-iphone-15-drfone-by-drfone-ios/"><u>Remove Device Supervision From your Apple iPhone 15 | Dr.fone</u></a></li>
<li><a href="https://extra-approaches.techidaily.com/revolutionize-your-podcast-with-these-ai-name-makers-for-2024/"><u>Revolutionize Your Podcast with These AI Name Makers for 2024</u></a></li>
<li><a href="https://techidaily.com/simple-ways-to-get-recent-calls-back-from-k11-5g-by-fonelab-android-recover-call-logs/"><u>Simple ways to get recent calls back from K11 5G</u></a></li>
<li><a href="https://buynow-help.techidaily.com/the-ultimate-guide-to-choosing-a-top-quality-budget-friendly-case-for-your-macbook-pro-13-a-review-of-finties-offering/"><u>The Ultimate Guide to Choosing a Top-Quality, Budget-Friendly Case for Your MacBook Pro 13: A Review of Fintie's Offering</u></a></li>
<li><a href="https://buynow-help.techidaily.com/the-ultimate-guide-to-choosing-an-office-chair-featuring-the-x-chair-x4/"><u>The Ultimate Guide to Choosing an Office Chair: Featuring the X-Chair X4</u></a></li>
<li><a href="https://buynow-help.techidaily.com/the-ultimate-guide-to-urban-armor-gears-durable-macbook-pro-protector/"><u>The Ultimate Guide to Urban Armor Gear's Durable MacBook Pro Protector</u></a></li>
<li><a href="https://techidaily.com/the-way-to-get-back-lost-call-history-from-itel-p55-5g-by-fonelab-android-recover-call-logs/"><u>The way to get back lost call history from Itel P55 5G</u></a></li>
<li><a href="https://buynow-help.techidaily.com/unboxing-and-evaluating-the-budget-friendly-tcl-50s425-a-2019-50-inch-4k-roku-television-review/"><u>Unboxing and Evaluating the Budget-Friendly TCL 50S425 - A 2019 50-Inch 4K Roku Television Review.</u></a></li>
<li><a href="https://buynow-help.techidaily.com/unveiling-the-lg-gram-156-an-extensive-review-of-a-remarkably-slim-and-long-lasting-ultrabook/"><u>Unveiling the LG Gram 15.6: An Extensive Review of a Remarkably Slim & Long-Lasting Ultrabook</u></a></li>
<li><a href="https://buynow-help.techidaily.com/unveiling-the-performance-of-genius-widecam-f10er-examining-pixelation-and-sound-quality-concerns/"><u>Unveiling the Performance of Genius WideCam F10er: Examining Pixelation & Sound Quality Concerns</u></a></li>
</ul></div>
