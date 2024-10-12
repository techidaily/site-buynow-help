---
title: "From Idea to Execution: Creating a Game Using ChatGPT's Assistance – The Full Story"
date: 2024-10-06T19:27:03.613Z
updated: 2024-10-12T17:00:48.830Z
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
<span id="1424528">
					<video width="864" height="1536" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1424528.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/16446-1424528">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1424528.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:540px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Flaganoo.pxf.io%2Fc%2F5597632%2F1424528%2F16446'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1424528/16446" style="position:absolute;visibility:hidden;" border="0" />
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

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2006955/19272" target="_top" id="2006955">
  <img src="//a.impactradius-go.com/display-ad/19272-2006955" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2006955/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

###  ChatGPT Is Far From Perfect

 LLMs are only as good (or as bad) as the prompts the user gives them. For example, a user could easily [generate anime-type characters with MidJourney](https://some-tips.techidaily.com/new-ultimate-strategies-pinterest-to-mp3-migration-guide/) by including a few words to clarify the prompt's end result. However, when building a game with ChatGPT, I found that there were times when the engine simply didn't pick up what I was putting down.

![An error happens that I can't seem to figure out, so I ask GPT for help](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/a-wild-unexpected-behavior-appears.png) 

 In this example, I encountered an issue with spawning my projectiles, with all the "bullets" being deflected when the player moves. While this could create some interesting play patterns, I decided to ask it to fix the problem, and it suggested a fix. Unfortunately, the fix didn't work.

![GPT's responses doesn't fix the error I keep having](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/the-error-is-still-there.png) 

 I eventually fixed it myself, but it highlighted a major issue with using ChatGPT to code a game: there are some things it doesn't know.

![A Do-it-Yourself Fix For The Programming Problem](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/diy-fix.png) 

 I eventually put together the game using a few suggestions from GPT about the persistent score as well as the random generation algorithm and scrolling for the game background. You can [play the final game here](https://zandoliearts.itch.io/the-unfriendly-skies).

<!-- affiliate ads begin -->
<a href="https://unicoeye.pxf.io/c/5597632/2134227/18498" target="_top" id="2134227">
  <img src="//a.impactradius-go.com/display-ad/18498-2134227" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://unicoeye.pxf.io/i/5597632/2134227/18498" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Does It Work With Other Game Engines?

 I know ChatGPT was very good with Unity once I could sort out some of the issues I ran into above. However, I wondered how coding a game with ChatGPT would work for a less-popular engine like Godot. I'm not exactly an expert in Godot, having used it far less than I did Unity. I decided to ask ChatGPT a few questions:

![GPT gives me a piece of code that is outdated because of GPT's limitations](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/gpt-s-godot-problem-1.png) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2105867/7443" target="_top" id="2105867">
  <img src="//a.impactradius-go.com/display-ad/7443-2105867" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2105867/7443" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://aligracehair.sjv.io/c/5597632/1934292/19272" target="_top" id="1934292">
  <img src="//a.impactradius-go.com/display-ad/19272-1934292" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1934292/19272" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://screen-activity-recording.techidaily.com/updated-2024-approved-comprehensive-list-best-10-terraria-mods/"><u>[Updated] 2024 Approved Comprehensive List Best 10 Terraria Mods</u></a></li>
<li><a href="https://screen-video-capture.techidaily.com/updated-2024-approved-navigate-nature-androids-animated-adventure-series/"><u>[Updated] 2024 Approved Navigate Nature Android’s Animated Adventure Series</u></a></li>
<li><a href="https://some-skills.techidaily.com/updated-unleash-creative-freedom-crafting-your-own-insta-tones/"><u>[Updated] Unleash Creative Freedom Crafting Your Own Insta Tones</u></a></li>
<li><a href="https://some-guidance.techidaily.com/2024-approved-the-compreayer-guide-to-iphone-hdr-mastery/"><u>2024 Approved The Compreayer Guide to iPhone HDR Mastery</u></a></li>
<li><a href="https://program-issues.techidaily.com/complete-rainbow-six-siege-debugging-eradicating-error-code-e-3-0x0001000b/"><u>Complete Rainbow Six Siege Debugging: Eradicating Error Code E 3-0X0001000B</u></a></li>
<li><a href="https://buynow-help.techidaily.com/exploring-the-imac-with-m1-stunning-display-and-impressive-performance/"><u>Exploring the iMac with M1: Stunning Display & Impressive Performance</u></a></li>
<li><a href="https://buynow-help.techidaily.com/exploring-the-sound-spectrum-with-nest-audio-perfect-harmony-for-melody-aficionados/"><u>Exploring the Sound Spectrum with Nest Audio: Perfect Harmony for Melody Aficionados</u></a></li>
<li><a href="https://buynow-help.techidaily.com/furbo-spotlight-celebrating-the-pinnacle-in-canine-surveillance-technology/"><u>Furbo Spotlight: Celebrating the Pinnacle in Canine Surveillance Technology</u></a></li>
<li><a href="https://buynow-help.techidaily.com/how-the-havit-5-way-gaming-laptop-cooler-transforms-overheating-issues/"><u>How the HAVIT 5-Way Gaming Laptop Cooler Transforms Overheating Issues</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/how-to-take-portrait-photo-with-old-iphone-x8-plus7-plus-for-2024/"><u>How to Take Portrait Photo with Old iPhone X/8 Plus/7 Plus for 2024</u></a></li>
<li><a href="https://location-social.techidaily.com/in-2024-proven-ways-in-how-to-hide-location-on-life360-for-honor-magic-vs-2-drfone-by-drfone-virtual-android/"><u>In 2024, Proven Ways in How To Hide Location on Life360 For Honor Magic Vs 2 | Dr.fone</u></a></li>
<li><a href="https://buynow-help.techidaily.com/in-depth-analysis-and-evaluation-xp-pen-artist-16-pro-graphic-tablet-unveiled/"><u>In-Depth Analysis and Evaluation: XP-Pen Artist 16 Pro Graphic Tablet Unveiled</u></a></li>
<li><a href="https://buynow-help.techidaily.com/in-depth-look-at-googles-pixelbook-go-top-notch-chrome-experience-for-a-hefty-price-tag/"><u>In-Depth Look at Google's Pixelbook Go: Top-Notch Chrome Experience for a Hefty Price Tag</u></a></li>
<li><a href="https://buynow-help.techidaily.com/lamicall-s-tablet-stand-review/"><u>Lamicall S Tablet Stand Review</u></a></li>
<li><a href="https://buynow-help.techidaily.com/linksys-wrt3200acm-router-review/"><u>Linksys WRT3200ACM Router Review</u></a></li>
<li><a href="https://buynow-help.techidaily.com/madden-nfl-19-critique-amazing-gameplay-aspects-facing-some-ageing-issues/"><u>Madden NFL 19 Critique: Amazing Gameplay Aspects Facing Some Ageing Issues</u></a></li>
<li><a href="https://smart-video-editing.techidaily.com/new-2024-approved-mts-video-editing-software-review-top-5-contenders/"><u>New 2024 Approved MTS Video Editing Software Review Top 5 Contenders</u></a></li>
<li><a href="https://extra-hints.techidaily.com/wintry-wonderland-olympic-moments-from-beijing-2022/"><u>Wintry Wonderland Olympic Moments From Beijing 2022</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/xbox-game-memories-save-them-with-screenshots-for-2024/"><u>Xbox Game Memories, Save Them with Screenshots for 2024</u></a></li>
</ul></div>

