---
title: How Does the Anti-Cheat Feature in Windows 11 Affect Gameplay Speeds and PC Efficiency?
date: 2024-08-27 19:19:14
updated: 2024-08-29 10:48:31
tags:
  - deals
categories:
  - tech
thumbnail: https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2021/12/powerful-personal-gaming-computer.jpg
---

## How Does the Anti-Cheat Feature in Windows 11 Affect Gameplay Speeds and PC Efficiency?

### Key Takeaways

* Virtualization-based security (VBS) enhances system security by creating an isolated environment for running security solutions, but it comes with some performance overhead.
* Gamers may be concerned about the impact of VBS on game performance, especially if they have hardware that just meets minimum requirements.
* Testing with the 3DMark Time Spy benchmark showed a small performance difference with VBS on versus off, particularly in CPU-limited scenarios, but the real-world impact was negligible and not noticeable in gameplay. It's generally recommended to leave VBS on for the security benefits.

 Virtualization-based security (VBS) has become a staple in the IT world for safeguarding systems. Yet, for gamers, the question isn't just about security but performance. So, does enabling VBS on Windows 11 actually slow down PC games? Let's find out.

##  What Is Virtualization-Based Security (VBS)?

 Before diving into the impact on gaming, it's important to understand what VBS actually is. Virtualization-based security uses hardware and software [virtualization](https://fox-direct.techidaily.com/new-different-editions-of-windows-film-editor-software-for-2024/) to enhance the security of a system. It essentially creates an isolated environment, separate from the operating system, where it can run various security solutions.

 By isolating software from the host system, you can prevent malicious or accidental damage. It's like running each app in its own little fish tank and carefully managing any interaction it has with hardware or other applications.

 The downside of this is that virtualization comes with some degree of overhead. In other words, processing power that could have gone to running the application faster is now going to managing the virtualization process. That being said, modern computers are designed at the hardware level with virtualization in mind, so the actual performance difference should be minimal in theory.

##  Why Gamers Should Care About VBS

 The prospect of sacrificing even a small percentage of performance can make gamers wary. After all, when you're in the heat of a virtual battle, [every frame per second (FPS) counts](https://tiktok-videos.techidaily.com/unleash-potential-in-tiktok-videos-free-editors-for-mac/). Additionally, some gaming rigs run on hardware that just meets the minimum system requirements. In such cases, even minor performance drops can make a noticeable difference.

 As mentioned above, virtualization inherently comes with some measure of system overhead that could be going towards video game performance. So, we expect to see some sort of performance difference with VBS on versus off, but how large is the impact?

##  How We Tested VBS' Impact on Windows 11

 I have a decent workstation laptop with a 24-core Intel 13900HX CPU and a laptop RTX 4060\. My goal is to determine if VBS makes any meaningful difference to my computer, but I encourage you to perform the following tests yourself because every system is different.

 To make 100% sure that no virtualization features could interfere with the results, I disabled virtualization in my laptop's BIOS. I also went to "Turn Windows Features On or Off" in the Control Panel and ensured that [Hyper-V](https://instagram-video-recordings.techidaily.com/in-2024-innovative-igtv-editor-apps-for-creative-vertical-content/) was disabled. Furthermore, I checked in the Group Policy Editor under Computer Configuration > Administrative Templates > System > Device Guard that VBS was disabled.

 While it makes sense to test for performance differences in gameplay, it's hard to get repeatable results, especially when the performance difference might be small, so I opted to use the popular 3DMark Time Spy synthetic benchmark instead. I ran the benchmark under the same conditions, apart from having virtualization on and off.

 3DMark has various benchmark tests that stress computers in different ways. Time Spy is a good test of mainstream gaming performance for modern games. The final score is calculated after taking various metrics into account across the whole system, and will tell us where our performance differences are coming from, rather than just telling us that it's better or worse.

##  The Results of Using VBS on Windows 11

 First, here are the results of running the benchmark with VBS on. We get a total system score of 11,028 and the graphics card gets a score of 10,478 points.

![VBS On 11 028 3D Mark Points](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/10/vbs-on.png) 

 Next, we have the results with VBS off after a restart. Now we get 11,125 for the overall score and the graphics score has gone up to 10,515.

![3D Mark VBS Off Score 11 125](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/10/2-21.png) 

 Clearly, the score with VBS off is higher, so we can say that VBS has some measure of performance impact. However, the difference in scores is so small that it wouldn't make a noticeable difference in gameplay.

 I ran the Time Spy benchmark three times with VBS on and with it off. There were no anomalies—the results were almost exactly the same in each test.

 However, if we look at the sub-scores, there may be more to it than that. While the graphics scores (which pertain to GPU performance) are virtually unchanged, the CPU score has a 5.3% difference: 15,706 versus 16,581\. Though, since 3DMark scores are scaled up by being multiplied by a constant, this score gap may be a little exaggerated.

 That said, this suggests that in CPU-limited scenarios (the [CPU's performance limits the frame rate](https://tech-recovery.techidaily.com/troubleshooting-windows-11-what-to-do-if-your-system-fails-to-shut-down/)), like eSports, turning VBS off might actually have a worthwhile performance boost—when we're talking about 100s of frames, a small amount of additional performance counts.

 This difference also suggests that anyone with older CPUs that have fewer cores (e.g., quad or hexacore CPUs) might have a proportionally larger impact compared to my 24-core system.

 That said, I played some _Cyberpunk 2077_ and noticed zero noticeable difference in real-world performance. If it ran any better with VBS off, I certainly couldn't tell.

 3D Mark scores are calculated using a weighted formula (per [UL.com](https://support.benchmarks.ul.com/support/solutions/articles/44002136143-how-is-the-3dmark-time-spy-score-calculated)) and are not directly comparable to, for example, the frame rate of a specific game. Despite this, making any changes to a system will affect the final score and frame rate is one of the components.

##  Who Should Disable VBS?

 In general, I recommend that anyone with a modern computer running Windows 11 should leave VBS on, since the security benefits outweigh the small performance penalty. However, you might decide to disable VBS if you:

* Don't have mission-critical data on your computer.
* Practice good digital safety when it comes to avoiding malware.
* Play CPU-bound eSports titles.
* Have a CPU that's close to the minimum level of performance already.

 It's easy enough to enable VBS again, so don't worry if you change your mind.

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
