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


