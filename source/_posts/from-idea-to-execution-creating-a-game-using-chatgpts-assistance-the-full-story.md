---
title: "From Idea to Execution: Creating a Game Using ChatGPT's Assistance – The Full Story"
date: 2024-10-29T05:03:57.220Z
updated: 2024-10-29T18:21:16.707Z
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

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2105876/7443" target="_top" id="2105876">
  <img src="//a.impactradius-go.com/display-ad/7443-2105876" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2105876/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 It's quickly apparent that GPT's willingness to [teach you to code](https://fox-helps.techidaily.com/navigating-gif-storage-and-use-in-the-digital-age-iphone/) a game is well-meaning but requires you to understand a bit about what you're doing. As someone who's been an amateur game developer for more than a decade, I know a little bit about coding a game. In using GPT to help me, I was interested in seeing how sophisticated it was for producing a playable game prototype.

###  It Certainly Understands Game Engines

 A game engine is what a developer uses to create a game. Several game engines are available, including [Unreal Engine](https://www.unrealengine.com/en-US), [Godot](https://godotengine.org/), and [Unity](https://unity.com/). As someone who knows Unity well, I decided to use this as my development engine. I asked a few general questions (that I know the answer to) to ensure that [ChatGPT wouldn't start hallucinating](https://audio-shaping.techidaily.com/strategies-for-minimizing-large-scale-video-and-audio-data/) about my game engine.

![ChatGPT describes the steps in building a player character](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/chatgpt-seems-to-know-some-stuff-1.png) 

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

 I eventually fixed it myself, but it highlighted a major issue with using ChatGPT to code a game: there are some things it doesn't know.

![A Do-it-Yourself Fix For The Programming Problem](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/diy-fix.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1915825/19272" target="_top" id="1915825">
  <img src="//a.impactradius-go.com/display-ad/19272-1915825" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1915825/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 I eventually put together the game using a few suggestions from GPT about the persistent score as well as the random generation algorithm and scrolling for the game background. You can [play the final game here](https://zandoliearts.itch.io/the-unfriendly-skies).

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2087239/19272" target="_top" id="2087239">
  <img src="//a.impactradius-go.com/display-ad/19272-2087239" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2087239/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Does It Work With Other Game Engines?

 I know ChatGPT was very good with Unity once I could sort out some of the issues I ran into above. However, I wondered how coding a game with ChatGPT would work for a less-popular engine like Godot. I'm not exactly an expert in Godot, having used it far less than I did Unity. I decided to ask ChatGPT a few questions:

![GPT gives me a piece of code that is outdated because of GPT's limitations](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/gpt-s-godot-problem-1.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1886015/19272" target="_top" id="1886015">
  <img src="//a.impactradius-go.com/display-ad/19272-1886015" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1886015/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

GPT's Godot Problem

 For those who use Godot regularly, the issue is immediately obvious. ChatGPT stopped learning in 2021 or thereabouts (at least for the free version). The script GPT gave me was based on its knowledge of Godot 2.x, which is a heavily outdated version of the current 4.x version. The glaring problem is the use of KinematicBody2D, which was replaced by CharacterBody2D in later iterations of the language.

##  How Much Skill Do You Need to Code a Game With ChatGPT?

 If you're considering making the next Legend of Zelda: Breath of the Wild using ChatGPT, you should probably temper your expectations. You need to have a decent understanding of the engine you're working in to use ChatGPT as a coding assistant.

 Other assistants like Microsoft Copilot might be better with general code and could help to a greater degree. The big issue is that these LLMs are looking at an abstract problem, and they're seeing it without actually seeing it.

 In simpler language, you know what the game you're making should look like and how things in it should behave. You can explain it to ChatGPT what you want, and it will give you something close to (but not quite) what your game needs. To make it behave the way you want it to, you'll have to fiddle around with the code that GPT gives you.

##  Should You Code a Game With ChatGPT?

![Screenshot of My Game's Title Page](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/screen-1-1.jpg) 

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
<li><a href="https://facebook-clips.techidaily.com/new-2024-approved-the-art-of-earning-money-with-your-facebook-page/"><u>[New] 2024 Approved The Art of Earning Money with Your Facebook Page</u></a></li>
<li><a href="https://youtube-stream.techidaily.com/new-step-by-step-guide-to-producing-quality-mobile-videos/"><u>[New] Step-by-Step Guide to Producing Quality Mobile Videos</u></a></li>
<li><a href="https://youtube-docs.techidaily.com/ed-in-2024-zenith-of-zest-elevate-with-elite-yoga-videos/"><u>[Updated] In 2024, Zenith of Zest Elevate with Elite Yoga Videos</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-in-depth-analysis-of-lgs-latest-360-cameras-for-the-year-2023/"><u>[Updated] In-Depth Analysis of LG's Latest 360 Cameras for the Year 2023</u></a></li>
<li><a href="https://buynow-help.techidaily.com/agptek-a01t-review/"><u>AGPTEK A01T Review</u></a></li>
<li><a href="https://buynow-help.techidaily.com/designed-for-success-a-closer-look-at-the-functional-lamicall-s-tablet-support-revealed/"><u>Designed for Success: A Closer Look at the Functional Lamicall S Tablet Support Revealed</u></a></li>
<li><a href="https://buynow-help.techidaily.com/exploring-the-shadowy-realms-of-bloodborne-an-immersive-review/"><u>Exploring the Shadowy Realms of Bloodborne - An Immersive Review</u></a></li>
<li><a href="https://tech-renaissance.techidaily.com/how-to-overcome-magic-mouse-movement-errors-effortlessly/"><u>How to Overcome Magic Mouse Movement Errors Effortlessly</u></a></li>
<li><a href="https://change-location.techidaily.com/how-to-watch-hulu-outside-us-on-honor-magic-6-drfone-by-drfone-virtual-android/"><u>How to Watch Hulu Outside US On Honor Magic 6 | Dr.fone</u></a></li>
<li><a href="https://change-location.techidaily.com/in-2024-pokemon-go-error-12-failed-to-detect-location-on-vivo-x100-pro-drfone-by-drfone-virtual-android/"><u>In 2024, Pokemon Go Error 12 Failed to Detect Location On Vivo X100 Pro? | Dr.fone</u></a></li>
<li><a href="https://buynow-help.techidaily.com/paww-audio-enlightenment-the-budget-friendly-review-of-series-3/"><u>Paww Audio Enlightenment - The Budget-Friendly Review of Series 3</u></a></li>
<li><a href="https://buynow-help.techidaily.com/samsung-galaxy-watch-active-2-an-in-depth-review-showcasing-upgraded-control-superior-connection-and-insight-features-over-original/"><u>Samsung Galaxy Watch Active 2: An In-Depth Review Showcasing Upgraded Control, Superior Connection & Insight Features Over Original.</u></a></li>
<li><a href="https://buynow-help.techidaily.com/seamless-connectivity-on-the-move-experience-unmatched-comfort-with-the-moko-universal-portable-bluetooth-keypad/"><u>Seamless Connectivity on The Move: Experience Unmatched Comfort with the MoKo Universal Portable Bluetooth Keypad</u></a></li>
<li><a href="https://extra-lessons.techidaily.com/the-photographers-companion-to-master-color-correction-top-11/"><u>The Photographer's Companion to Master Color Correction (Top 11)</u></a></li>
<li><a href="https://android-location-track.techidaily.com/top-5-tracking-apps-to-track-poco-x5-without-them-knowing-drfone-by-drfone-virtual-android/"><u>Top 5 Tracking Apps to Track Poco X5 without Them Knowing | Dr.fone</u></a></li>
<li><a href="https://buynow-help.techidaily.com/top-rated-rechargeable-battery-chargers-in-2e-the-ultimate-list/"><u>Top-Rated Rechargeable Battery Chargers in 2E: The Ultimate List</u></a></li>
<li><a href="https://buynow-help.techidaily.com/unveiling-the-powerhouse-a-deep-dive-into-the-new-samsung-galaxy-s2-ultra-features-and-performance/"><u>Unveiling the Powerhouse: A Deep Dive Into the New Samsung Galaxy S2# Ultra Features & Performance</u></a></li>
</ul></div>

