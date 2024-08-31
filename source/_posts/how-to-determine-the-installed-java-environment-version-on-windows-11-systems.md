---
title: How to Determine the Installed Java Environment Version on Windows 11 Systems
date: 2024-08-30T09:04:02.210Z
updated: 2024-08-31T09:04:02.210Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/52687750468_dc6bdda141_o-15.jpg
---

## How to Determine the Installed Java Environment Version on Windows 11 Systems

### Quick Links

* [Check Your Java Version Graphically](https://article-tips.techidaily.com/2024-approved-taking-photos-and-posting-youtubes-complete-guidebook/)
* [Check Your Java Version Using the Command Prompt](https://mondly-stories.techidaily.com/unearthing-millennia-old-linguistic-foundations/)
* [Check Your Java Version Using PowerShell](https://fox-access.techidaily.com/new-in-2024-the-art-of-chromatic-enhancement/)

### Key Takeaways

* You can check your Java version graphically by searching for "About Java" or "Configure Java" in the Start menu and clicking the top result.
* If you want to check your Java version in a command-line interface, open Command Prompt or PowerShell, then enter "java -version" in the console.

 Some apps require you to run a certain Java version to properly function. You can check which version of Java you have installed using a graphical tool or via the command line.

##  Check Your Java Version Graphically

 If you prefer to avoid the command line, you can use the About Java utility to find the installed Java version.

 To use this method, open the "Start" menu, search for "About Java," then click the first result.

![Searching "About Java" in the Start menu.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/1-search-about-java.png) 

<!-- affiliate ads begin -->
<a href="https://shop.mondly.com/affiliate.php?ACCOUNT=ATISTUDI&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.mondly.com%3FAFFILIATE%3D108875%26RESOURCE%3D%2BGeneral%2B970x90%2B"><img src="https://secure.avangate.com/images/merchant/69c418c33ec2e1a4267fa9bb77fa1428/general-970x90.gif" border="0"></a>
<!-- affiliate ads end -->
 Here, you'll see your current Java version listed in the first line.

![The Java version window.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/2-java-version.png) 

 If you don't see About Java in the Start menu, search for "Configure Java" instead and click it. Then click "About" to see your Java version.

 If you don't see either the About Java or Configure Java tools, you likely don't have Java installed. You can [download it](https://www.java.com/en/download/) from Oracle's official website.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=3727260&QTY=1&AFFILIATE=108875&CART=1"><img src="http://www.aiseesoft.com/avangate/30p/banner.jpg" border="0"></a>
<!-- affiliate ads end -->
##  Check Your Java Version Using the Command Prompt

 You can check your Java version from the Command Prompt, too.

 To begin, open the Start menu, search for "Command Prompt," then click the "Command Prompt" shortcut in the search results.

![Search for 'Command Prompt' in the Start menu.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/3-search-command-prompt.png) 

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4713565&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.epubor.com/images/uppic/audible-converter-interface.png" border="0">Epubor Audible Converter for Mac： Download and convert Audible AAXC/AA/AAX to MP3 with 100% original quality preserved.</a>
<!-- affiliate ads end -->
 When the Command Prompt opens, type the following command at the prompt and press "Enter."

java -version

 You'll see "java version" and some numbers next to it. These numbers are your Java version.

![The output of 'java -version' in Command Prompt.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/4-java-version-in-command-prompt.png) 

 If the Command Prompt says that Java is not recognized as an internal or external command, that's probably because the system variables are not properly set---or perhaps because you don't have Java installed. Reinstall Java on your PC and this should fix the issue for you.

<!-- affiliate ads begin -->
<a href="https://vapordna.pxf.io/c/5597632/1496243/17238" target="_top" id="1496243"><img src="//a.impactradius-go.com/display-ad/17238-1496243" border="0" alt="" width="1000" height="1221"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1496243/17238" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
##  Check Your Java Version Using PowerShell

 Checking your Java version in PowerShell is basically the same as Command Prompt. First, open the Start menu and search "powershell," then click the top result to launch PowerShell. 

![Search 'PowerShell' in the Start menu.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/powershell.png) 

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=36506229&QTY=1&AFFILIATE=108875&CART=1"><video width="100%" height="" class="rounded-t-md shadow-lg relative z-20" controls="" autoplay="" loop="" muted="" playsinline="" webkit-playinginline="">
<source type="video/mp4" src="https://aidaform.com/images/videos/aidaform-welcome-site.mp4"><source type="video/webm" src="https://aidaform.com/images/videos/aidaform-welcome-site.webm"></video></a>
<!-- affiliate ads end -->
 Type **java -version** into the window and hit Enter. Information about your Java version will be dispayed below.

![5 java version in powershell](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/5-java-version-in-powershell.png) 

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=3922934&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/4b0a0290ad7df100b77e86839989a75e/products/ripperpro.png" border="0">WonderFox DVD Ripper Pro</a>
<!-- affiliate ads end -->
Information about Java displayed in PowerShell. 

 It is important to note that this only shows you the version of Java you have on your [system PATH](https://android-frp.techidaily.com/in-2024-the-complete-guide-to-meizu-frp-bypass-everything-you-need-to-know-by-drfone-android/). It is possible to have multiple versions of Java installed concurrently, but this command will only display one. 

---

 If you use Ubuntu alongside Windows, there's a command that you can use to [check whether Java is installed on your Ubuntu-based computer](https://screen-recording.techidaily.com/updated-2024-approved-economical-android-communication-tools-best-of-10/). And if it's not, you can install it fairly easily.

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
<li><a href="https://youtube-lab.techidaily.com/harting-a-course-for-revenue-with-ytp2024-insights/"><u>[New] Charting a Course for Revenue with YTP2024 Insights</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/new-in-depth-analysis-of-premium-apps-to-boost-vtuber-audibility/"><u>[New] In-Depth Analysis of Premium Apps to Boost Vtuber Audibility</u></a></li>
<li><a href="https://extra-approaches.techidaily.com/new-pixlr-essentials-10-pro-tips-to-transform-your-images/"><u>[New] Pixlr Essentials  10 Pro Tips to Transform Your Images</u></a></li>
<li><a href="https://screen-activity-recording.techidaily.com/new-unlocking-ppts-potential-with-voiceover-techniques/"><u>[New] Unlocking PPT's Potential with Voiceover Techniques</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/updated-from-frame-to-phrase-expertly-ranked-29-video-translators-on-the-market/"><u>[Updated] From Frame to Phrase  Expertly Ranked 29 Video Translators on the Market</u></a></li>
<li><a href="https://youtube-docs.techidaily.com/ed-in-2024-monetizing-your-youtube-channels-strategies-for-success/"><u>[Updated] In 2024, Monetizing Your YouTube Channels  Strategies for Success</u></a></li>
<li><a href="https://youtube-stream.techidaily.com/2024-approved-finding-your-voice-on-youtube-a-guide-to-selective-audiences/"><u>2024 Approved  Finding Your Voice on YouTube  A Guide to Selective Audiences</u></a></li>
<li><a href="https://extra-approaches.techidaily.com/2024-approved-mastering-windows-11-wallpaper-upgrade-tips/"><u>2024 Approved  Mastering Windows 11  Wallpaper Upgrade Tips</u></a></li>
<li><a href="https://article-tips.techidaily.com/2024-approved-ultimate-guide-to-top-sierra-dvd-makers/"><u>2024 Approved  Ultimate Guide to Top Sierra DVD Makers</u></a></li>
<li><a href="https://facebook-videos.techidaily.com/2024-approved-what-you-must-watch-a-close-look-at-todays-top-8-social-media-clips/"><u>2024 Approved  What You Must Watch! - A Close Look at Today's Top 8 Social Media Clips</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/discovering-windows-10-release-information-a-guide-to-finding-your-systems-build-number/"><u>Discovering Windows 10 Release Information: A Guide to Finding Your System's Build Number</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/easy-tips-to-update-and-download-essential-software-for-your-hp-envy-ebx-series-computer/"><u>Easy Tips to Update & Download Essential Software for Your HP ENVY Ebx Series Computer</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/enter-safe-mode-in-windows-8-and-81-easily/"><u>Enter Safe Mode in Windows 8 & 8.1. Easily!</u></a></li>
<li><a href="https://win-howtos.techidaily.com/fixing-the-failure-of-touchpad-scrolling-functionality-in-windows-10/"><u>Fixing the Failure of Touchpad Scrolling Functionality in Windows 10</u></a></li>
<li><a href="https://screen-sharing-recording.techidaily.com/from-amateurs-to-pros-mastering-mac-audio-in-audacity-for-2024/"><u>From Amateurs to Pros  Mastering Mac Audio in Audacity for 2024</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/getting-started-with-action-cams-latest-2023-insights-for-2024/"><u>Getting Started with Action Cams – Latest 2023 Insights for 2024</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/guide-mastering-the-art-of-snapping-screenshots-with-windows/"><u>Guide: Mastering the Art of Snapping Screenshots with Windows ✨🖥️</u></a></li>
<li><a href="https://activate-lock.techidaily.com/how-to-bypass-activation-lock-on-iphone-6s-or-ipad-by-drfone-ios/"><u>How to Bypass Activation Lock on iPhone 6s or iPad?</u></a></li>
<li><a href="https://location-social.techidaily.com/how-to-changeadd-location-filters-on-snapchat-for-your-samsung-galaxy-f34-5g-drfone-by-drfone-virtual-android/"><u>How to Change/Add Location Filters on Snapchat For your Samsung Galaxy F34 5G | Dr.fone</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/how-to-fix-windows-10-creators-update-downloading-and-audio-problems/"><u>How to Fix Windows 10 Creator's Update Downloading and Audio Problems</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/how-to-fix-windows-10-insider-preview-build-15031-when-downloading-gets-stuck-on-initialization/"><u>How to Fix Windows 10 Insider Preview Build 15031 When Downloading Gets Stuck on Initialization</u></a></li>
<li><a href="https://techidaily.com/how-to-hard-reset-zte-nubia-flip-5g-without-password-drfone-by-drfone-reset-android-reset-android/"><u>How to Hard Reset ZTE Nubia Flip 5G Without Password | Dr.fone</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/how-to-overcome-unable-to-run-files-in-temp-directory-and-complete-initialization-successfully/"><u>How to Overcome 'Unable to Run Files in Temp Directory' And Complete Initialization Successfully</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/how-to-remove-quick-access-in-windows-10/"><u>How to Remove Quick Access in Windows 10</u></a></li>
<li><a href="https://win-amazing.techidaily.com/how-to-update-your-techkey-bluetooth-adapter-with-newest-drivers-on-windows-systems-win11-win7-win8/"><u>How to Update Your Techkey Bluetooth Adapter with Newest Drivers on Windows Systems (Win11, Win7, Win8)</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/in-2024-frame-perfect-our-top-10-photo-lenses-list/"><u>In 2024, Frame Perfect  Our Top 10 Photo Lenses List</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/in-2024-fresh-selection-of-engagement-prompts-for-audio-audiences/"><u>In 2024, Fresh Selection of Engagement Prompts for Audio Audiences</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/in-2024-from-ground-to-sky-the-lifting-elite-drone-list/"><u>In 2024, From Ground to Sky  The Lifting Elite Drone List</u></a></li>
<li><a href="https://digital-screen-recording.techidaily.com/in-2024-unmatched-visuals-leading-ps5-compatible-hdmi-21-monitors/"><u>In 2024, Unmatched Visuals  Leading PS5 Compatible HDMI 2.1 Monitors</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/instavideo-magic-crafting-a-plan-to-capture-your-audiences-attention-for-2024/"><u>InstaVideo Magic  Crafting a Plan to Capture Your Audience's Attention for 2024</u></a></li>
<li><a href="https://ai-driven-video-production.techidaily.com/new-in-2024-free-and-fantastic-the-best-mp4-video-editors/"><u>New In 2024, Free and Fantastic The Best MP4 Video Editors</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/notable-20-free-non-exclusive-pubg-screenshots-for-2024/"><u>Notable 20 Free, Non-Exclusive PUBG Screenshots for 2024</u></a></li>
<li><a href="https://extra-tips.techidaily.com/pioneering-computing-insights-from-toms-technology-review/"><u>Pioneering Computing Insights From Tom's Technology Review</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/resolving-issues-with-intel-serial-io-driver-on-non-compatible-systems/"><u>Resolving Issues with Intel Serial IO Driver on Non-Compatible Systems</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/simplifying-troubleshooting-the-ultimate-guide-to-clean-boots-in-windows-11/"><u>Simplifying Troubleshooting: The Ultimate Guide to Clean Boots in Windows 11</u></a></li>
<li><a href="https://tech-revival.techidaily.com/steer-clear-of-data-mining-with-chatgpt-exit/"><u>Steer Clear of Data Mining with ChatGPT Exit</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/step-by-step-guide-to-setting-up-system-protection-and-creating-a-restore-point-on-windows-10/"><u>Step-by-Step Guide to Setting Up System Protection and Creating a Restore Point on Windows 10</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/step-by-step-guide-setting-up-system-restore-on-your-pc-running-windows-10/"><u>Step-by-Step Guide: Setting Up System Restore on Your PC Running Windows 10</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/troubleshooting-and-solving-common-errors-in-the-windows-11-calculator-app/"><u>Troubleshooting and Solving Common Errors in the Windows 11 Calculator App</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/troubleshooting-guide-execution-failed-with-error-code-amoebadll-gain-access-now/"><u>Troubleshooting Guide: Execution Failed with Error Code amoeba.dll – Gain Access Now!</u></a></li>
<li><a href="https://program-issues.techidaily.com/troubleshooting-why-is-my-game-sifu-experiencing-fps-drops-and-stuttering-on-a-pc/"><u>Troubleshooting: Why Is My Game 'Sifu' Experiencing FPS Drops and Stuttering on a PC?</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/ultimate-guide-launching-admin-level-command-prompt-on-windows-10-8-and-81/"><u>Ultimate Guide: Launching Admin-Level Command Prompt on Windows 10, 8 & 8.1</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/ultimate-tutorial-accessing-and-launching-cmd-as-an-administrator-in-windows-11-8-and-81/"><u>Ultimate Tutorial: Accessing and Launching CMD as an Administrator in Windows 11, 8 & 8.1</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/windows-10-themes-personalize-your-pc/"><u>Windows 10 Themes: Personalize Your PC</u></a></li>
</ul></div>
