---
title: "From Idea to Execution: Creating a Game Using ChatGPT's Assistance – The Full Story"
date: 2024-12-28T16:01:40.263Z
updated: 2025-01-03T17:38:51.767Z
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

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/fHWdQw1gRyI?si=ve9wZnPupiooLThG" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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
<iframe width="560" height="315" src="https://www.youtube.com/embed/NC0rdKEQ98o?si=HYgqC8CxF_WTO5if" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

###  ChatGPT Is Far From Perfect

 LLMs are only as good (or as bad) as the prompts the user gives them. For example, a user could easily [generate anime-type characters with MidJourney](https://some-tips.techidaily.com/new-ultimate-strategies-pinterest-to-mp3-migration-guide/) by including a few words to clarify the prompt's end result. However, when building a game with ChatGPT, I found that there were times when the engine simply didn't pick up what I was putting down.

![An error happens that I can't seem to figure out, so I ask GPT for help](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/a-wild-unexpected-behavior-appears.png) 

 In this example, I encountered an issue with spawning my projectiles, with all the "bullets" being deflected when the player moves. While this could create some interesting play patterns, I decided to ask it to fix the problem, and it suggested a fix. Unfortunately, the fix didn't work.

![GPT's responses doesn't fix the error I keep having](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/the-error-is-still-there.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/jvwX82j3ci0?si=gAWoovjXgs3m1d7S" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 I eventually fixed it myself, but it highlighted a major issue with using ChatGPT to code a game: there are some things it doesn't know.

![A Do-it-Yourself Fix For The Programming Problem](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/diy-fix.png) 

 I eventually put together the game using a few suggestions from GPT about the persistent score as well as the random generation algorithm and scrolling for the game background. You can [play the final game here](https://zandoliearts.itch.io/the-unfriendly-skies).

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/iPCr_bxZjMQ?si=ubOsoq5umPEXL9xL" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Does It Work With Other Game Engines?

 I know ChatGPT was very good with Unity once I could sort out some of the issues I ran into above. However, I wondered how coding a game with ChatGPT would work for a less-popular engine like Godot. I'm not exactly an expert in Godot, having used it far less than I did Unity. I decided to ask ChatGPT a few questions:

![GPT gives me a piece of code that is outdated because of GPT's limitations](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/05/gpt-s-godot-problem-1.png) 

GPT's Godot Problem

 For those who use Godot regularly, the issue is immediately obvious. ChatGPT stopped learning in 2021 or thereabouts (at least for the free version). The script GPT gave me was based on its knowledge of Godot 2.x, which is a heavily outdated version of the current 4.x version. The glaring problem is the use of KinematicBody2D, which was replaced by CharacterBody2D in later iterations of the language.

##  How Much Skill Do You Need to Code a Game With ChatGPT?

 If you're considering making the next Legend of Zelda: Breath of the Wild using ChatGPT, you should probably temper your expectations. You need to have a decent understanding of the engine you're working in to use ChatGPT as a coding assistant.

 Other assistants like Microsoft Copilot might be better with general code and could help to a greater degree. The big issue is that these LLMs are looking at an abstract problem, and they're seeing it without actually seeing it.

 In simpler language, you know what the game you're making should look like and how things in it should behave. You can explain it to ChatGPT what you want, and it will give you something close to (but not quite) what your game needs. To make it behave the way you want it to, you'll have to fiddle around with the code that GPT gives you.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/HaM818fFKXQ?si=ZZLA4lFSHSgCpSE0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://vimeo-videos.techidaily.com/updated-in-2024-rapid-access-accelerating-vimeo-videos/"><u>[Updated] In 2024, Rapid Access Accelerating Vimeo Videos</u></a></li>
<li><a href="https://screen-sharing-recording.techidaily.com/updated-screen-savvy-taking-screenshots-on-windows-for-2024/"><u>[Updated] Screen Savvy Taking Screenshots on Windows for 2024</u></a></li>
<li><a href="https://buynow-help.techidaily.com/2024s-top-choices-premium-wrist-pads-for-enhanced-typing-ergonomics/"><u>2024’S Top Choices: Premium Wrist Pads for Enhanced Typing Ergonomics</u></a></li>
<li><a href="https://buynow-help.techidaily.com/a-close-look-at-star-wars-squadrons-experience-the-thrill-of-hyper-realistic-space-skirmishes/"><u>A Close Look At Star Wars Squadrons – Experience the Thrill of Hyper-Realistic Space Skirmishes!</u></a></li>
<li><a href="https://buynow-help.techidaily.com/a-detailed-analysis-and-user-reviews-of-the-newly-launched-ring-doorbell-pro-max/"><u>A Detailed Analysis & User Reviews of the Newly Launched Ring Doorbell Pro Max</u></a></li>
<li><a href="https://howto.techidaily.com/cellular-network-not-available-for-voice-calls-on-vivo-y17s-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>Cellular Network Not Available for Voice Calls On Vivo Y17s | Dr.fone</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/how-to-screen-mirroring-vivo-g2-to-pc-drfone-by-drfone-android/"><u>How to Screen Mirroring Vivo G2 to PC? | Dr.fone</u></a></li>
<li><a href="https://extra-tips.techidaily.com/mastering-brand-collaboration-on-youtube/"><u>Mastering Brand Collaboration on YouTube</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/seamless-file-interaction-discover-these-6-gpt-apps/"><u>Seamless File Interaction: Discover These 6 GPT Apps</u></a></li>
<li><a href="https://some-tips.techidaily.com/shared-frustrations-after-transitioning-to-iphone-ios-18-lessons-learned/"><u>Shared Frustrations After Transitioning to iPhone iOS 18 - Lessons Learned</u></a></li>
<li><a href="https://sim-unlock.techidaily.com/top-11-free-apps-to-check-imei-on-tecno-spark-10-5g-phones-by-drfone-android/"><u>Top 11 Free Apps to Check IMEI on Tecno Spark 10 5G Phones</u></a></li>
<li><a href="https://technical-tips.techidaily.com/top-4-standout-iphone-16-innovations-that-justify-an-upgrade-a-deep-dive-by-zdnet/"><u>Top 4 Standout iPhone 16 Innovations That Justify an Upgrade: A Deep Dive by ZDNet</u></a></li>
<li><a href="https://buynow-help.techidaily.com/unlocking-the-potential-of-budget-friendly-phones-with-a-moto-g-stylus-review/"><u>Unlocking the Potential of Budget-Friendly Phones with a Moto G Stylus Review</u></a></li>
<li><a href="https://buynow-help.techidaily.com/unpacking-the-strengths-of-nokias-72-a-comprehensive-look-at-a-mid-range-market-disruptor/"><u>Unpacking the Strengths of Nokia's 7.2: A Comprehensive Look at a Mid-Range Market Disruptor</u></a></li>
<li><a href="https://buynow-help.techidaily.com/unveiling-the-high-performance-capabilities-of-fujitsus-ix1600-document-scanner-desktop-review/"><u>Unveiling the High-Performance Capabilities of Fujitsu's iX1600 Document Scanner - Desktop Review</u></a></li>
<li><a href="https://buynow-info.techidaily.com/viair-88p-reviewed-a-robust-compressor-with-notable-exceptions-examined/"><u>Viair 88P Reviewed: A Robust Compressor with Notable Exceptions Examined</u></a></li>
<li><a href="https://buynow-help.techidaily.com/what-is-elgoog/"><u>What Is elgooG?</u></a></li>
<li><a href="https://buynow-help.techidaily.com/wireless-ears-delight-at-economic-prices-senso-buds/"><u>Wireless Ears' Delight at Economic Prices: Senso Buds</u></a></li>
<li><a href="https://buynow-help.techidaily.com/z7-review-nearly-perfect-practically-exceptional-photography/"><u>Z7 Review: Nearly Perfect, Practically Exceptional Photography</u></a></li>
</ul></div>

