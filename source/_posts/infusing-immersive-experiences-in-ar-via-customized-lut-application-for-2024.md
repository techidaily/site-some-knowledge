---
title: "Infusing Immersive Experiences in AR via Customized LUT Application for 2024"
date: 2024-08-21T12:54:18.526Z
updated: 2024-08-22T12:54:18.526Z
tags: 
  - screen-recording
  - ai video
  - ai audio
  - ai auto
categories: 
  - ai
  - screen
description: "This Article Describes Infusing Immersive Experiences in AR via Customized LUT Application for 2024"
excerpt: "This Article Describes Infusing Immersive Experiences in AR via Customized LUT Application for 2024"
keywords: "AR Immersion Tech,Custom LUT for AR,AR User Experience,LUT AR Designs,AR Personalization,Interactive AR Tools,LUT in AR Worlds"
thumbnail: https://thmb.techidaily.com/97b0ddc570e6ff11d98aa739ad9094bf8b6916f3ca7d54eab5f1d4007ba674c0.JPG
---

## Infusing Immersive Experiences in AR via Customized LUT Application

Color LUTs (Lookup Textures) are tables of RGB color values. In Spark AR, you can use color LUTs to quickly create color gradation effects throughout the scene. Go through the article and create your color LUT effect.

## Part 1\. What are Luts in Spark AR used for?

To create a color filter effect in [Spark AR](https://sparkar.facebook.com/ar-studio/), you need a color LUT in Spark AR.

To develop AR effects for mobile cameras, you can use the Mac and Windows augmented reality platform Spark AR Studio. Imagine it like Sketch or Photoshop for augmented reality. The color values of the camera texture are mapped to the x, y, and z coordinates of the location in the color LUT. This location contains a corresponding output color that is drawn over the scene to create a color gradient effect.

![create a color gradient effect](https://images.wondershare.com/filmora/article-images/2022/08/how-to-use-luts-in-spark-ar-1.jpg)

## Part 2\. How to use LUTs in Spark AR?

**How to apply a color LUT to the whole scene in Spark AR:**

##### Step1Add a color LUT to your project

1. In the Assets panel, click Add Asset.
2. Select Import, then Color LUT, and select your file from your computer.

When you import a color LUT, compression is always set to None, and filtering is set to Low by default.

##### Step2Apply to the whole scene

1. In the Assets panel, right-click the LUT color.
2. Select Actions and then **Apply to Camera**.

A patch graph is automatically set that applies a color LUT to the entire scene.

<!-- affiliate ads begin -->
<a href="https://ship7com.pxf.io/c/5597632/1509856/17634" target="_top" id="1509856"><img src="//a.impactradius-go.com/display-ad/17634-1509856" border="0" alt="" width="730" height="383"/></a>
<!-- affiliate ads end -->
![apply to the whole scene](https://images.wondershare.com/filmora/article-images/2022/08/how-to-use-luts-in-spark-ar-2.jpg)

**The color LUT patch graph**

The patch graph that renders the color gradation effect looks like this:

![color lut patch graph](https://images.wondershare.com/filmora/article-images/2022/08/how-to-use-luts-in-spark-ar-3.jpg)

**To create the effect:**

* Fix Scene Render Pass renders cameraTexture0 and all objects in the scene that are children of the device. This creates the output texture.
* ColorLUTShader looks up the RGBA values of this texture in the Tension color LUT array and converts them to a new green color. This will change the texture and create a gradient effect.
* Finally, the Screen Output patch renders the green color.

## Part 3\. Free LUTs resource for Spark AR

Here are the best free LUTs resources for Spark AR:

<!-- affiliate ads begin -->
<a href="https://tinyland.pxf.io/c/5597632/1793214/19135" target="_top" id="1793214"><img src="//a.impactradius-go.com/display-ad/19135-1793214" border="0" alt="" width="900" height="900"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1793214/19135" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
### 1\. [Frost Zombie (Technical Showcase)](https://we.tl/t-1uj4wJKluG)

Client filter pieces occasionally end up on the scrap heap. It was a poor Frost Zombie in this instance. Since this is one of my simpler filters, I felt it was okay to publish the build information. Four objects make up much of the scene: an EyeColor block, a custom canvas segmentation, a face mesh, and an emitter for the breath mist (my personal favorite). To show the layers used in generating the primary zombie texture, I also moved to Substance Painter. This is a demonstration of my methods rather than a step-by-step manual.

<!-- affiliate ads begin -->
<a href="https://versadesk.pxf.io/c/5597632/1892108/21290" target="_top" id="1892108"><img src="//a.impactradius-go.com/display-ad/21290-1892108" border="0" alt="" width="1080" height="1080"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1892108/21290" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![frost zombie](https://images.wondershare.com/filmora/article-images/2022/08/how-to-use-luts-in-spark-ar-4.jpg)

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=40085955&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/f702defbc67edb455949f46babab0c18/products/2_logo9.png" border="0">FX PRO (Gold Robot + Silver Robot(Basic Package))</a>
<!-- affiliate ads end -->
### 2\. Fur

Here are the key building principles.

* Geometric layers, often known as shells, produce depth.
* Normals is used to create shells from a single mesh.
* Alpha decreases with each shell.
* Deeper shells are darker.
* Height is generated from a single grayscale channel.
* No fur is generated in the black areas of the height texture.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=3922934&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/4b0a0290ad7df100b77e86839989a75e/products/ripperpro.png" border="0">WonderFox DVD Ripper Pro</a>
<!-- affiliate ads end -->
![fur](https://images.wondershare.com/filmora/article-images/2022/08/how-to-use-luts-in-spark-ar-5.jpg)

<!-- affiliate ads begin -->
<a href="https://getlyla.pxf.io/c/5597632/1455723/15391" target="_top" id="1455723"><img src="//a.impactradius-go.com/display-ad/15391-1455723" border="0" alt="" width="336" height="280"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1455723/15391" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
### 3\. Shockwave

Even while using large image sequences is frequently discouraged, you can still use them to make some extremely spectacular effects! I'll explain how the screen tap computation procedure relates to texture position in this walkthrough. If you want to apply this approach and texture sequence in your projects or give it a try.

<!-- affiliate ads begin -->
<a href="https://estore.winxdvd.com/order/checkout.php?PRODS=4612444&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.winxdvd.com/affiliate/new-banner/pt-728x90.jpg" border="0"></a>
<!-- affiliate ads end -->
![shockwave](https://images.wondershare.com/filmora/article-images/2022/08/how-to-use-luts-in-spark-ar-6.jpg)

### 4\. Transition Curves

There are 11 distinct animation curves included with Spark AR in the Transition patch. Here is a helpful visual aid because it might be challenging to distinguish between a quartic and a quintic when working on a project. With the SDF circle doubled (to sharpen the edge) and inserted into the Patch Pack's alpha channel, the circles are likewise straightforward rectangles. Since RGB values are three times one, the object is white.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4693127&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.videosoftdev.com/images/video_editor/screenshots/1.jpg" border="0">
VSDC Pro Video Editor is a light professional non-linear video editing suite for creating a movie of any complexity. It supports the most popular video/audio formats and codecs, including 4K, HD and GoPro videos. Preconfigured profiles make the creation of videos for various multimedia and mobile devices absolutely hassle-free.

Key features:

•	Import from any devices and cams, including GoPro and drones. All formats supported. Сurrently the only free video editor that allows users to export in a new H265/HEVC codec, something essential for those working with 4K and HD.
•	Everything for hassle-free basic editing: cut, crop and merge files, add titles and favorite music
•	Visual effects, advanced color correction and trendy Instagram-like filters   
•	All multimedia processing done from one app: video editing capabilities reinforced by  a video converter, a screen capture, a video capture, a disc burner and a YouTube uploader
•	Non-linear editing: edit several files with simultaneously 
•	Easy export to social networks: special profiles for YouTube, Facebook, Vimeo, Twitter and Instagram
•	High quality export – no conversion quality loss, double export speed even of HD files due to hardware acceleration
•	Stabilization tool will turn shaky or jittery footage into a more stable video automatically. 
•	Essential toolset for professional video editing: blending modes, Mask tool, advanced multiple-color Chroma Key  
</a>
<!-- affiliate ads end -->
![transition curves](https://images.wondershare.com/filmora/article-images/2022/08/how-to-use-luts-in-spark-ar-7.jpg)

### 5\. Realistic Smoke

By adding smoke to a scene, you can easily add a lot of detail and realism. Nothing revolutionary is happening here. The particle emitter creates flat planes of smoke texture that are forced upward. The force slowly shifts left and right as seen in the patch editor. The Fade particle script (created by Josh Beckwith) enlarges the particles and fades them out at the same time.

![realistic smoke](https://images.wondershare.com/filmora/article-images/2022/08/how-to-use-luts-in-spark-ar-8.jpg)

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=45152835&QTY=1&AFFILIATE=108875&CART=1"><img src="https://download.terabyteunlimited.com/banners/ad_800x450_d.jpg" border="0"></a>
<!-- affiliate ads end -->
### 6\. Rainbow Glitter

Given how beautifully Glitter Rain was received, I believed it would be fitting to broaden the potential with an HDR setting. While Glitter Rain made use of two different colors, this technique makes use of an entirely colorless substance and gets its color information via HDR.

![rainbow glitter](https://images.wondershare.com/filmora/article-images/2022/08/how-to-use-luts-in-spark-ar-9.jpg)

### Closing Thoughts

Spark AR is an amazing website for LUTs and color grading. Whether you're a new student or a seasoned pro, Spark AR Studio has all the features and capabilities you need to become a good video editor. You can download free LUTs from Spark AR and apply them to your videos. The article guides on how to use LUTs in Spark AR and how to download free LUTs. So, Spark AR is one of the best online websites for LUTs I have tried.

[Free Download](https://tools.techidaily.com/wondershare/filmora/download/)For Win 7 or later(64-bit)

[Free Download](https://tools.techidaily.com/wondershare/filmora/download/)For macOS 10.14 or later

[Free Download](https://tools.techidaily.com/wondershare/filmora/download/)For macOS 10.14 or later

<ins class="adsbygoogle"
     style="display:block"
     data-ad-format="autorelaxed"
     data-ad-client="ca-pub-7571918770474297"
     data-ad-slot="1223367746"></ins>

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
<li><a href="https://facebook-clips.techidaily.com/new-2024-approved-discover-the-next-wave-of-effective-facebook-ad-techniques/"><u>[New] 2024 Approved  Discover the Next Wave of Effective Facebook Ad Techniques</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/new-2024-approved-the-complete-guide-to-proficient-use-of-screenrec-software/"><u>[New] 2024 Approved  The Complete Guide to Proficient Use of ScreenRec Software</u></a></li>
<li><a href="https://desktop-recording.techidaily.com/new-2024-approved-whos-leading-in-screen-capture-tech-obs-studios-vs-bandicam/"><u>[New] 2024 Approved  Who's Leading in Screen Capture Tech  OBS Studios Vs. Bandicam</u></a></li>
<li><a href="https://youtube-web.techidaily.com/-comprehensive-guide-to-creating-viral-youtube-shorts-videos/"><u>[New] A Comprehensive Guide to Creating Viral YouTube Shorts Videos</u></a></li>
<li><a href="https://extra-information.techidaily.com/new-best-subtitle-converters-reviewed-the-top-8-win-osx-sbt-to-srts-software/"><u>[New] Best Subtitle Converters Reviewed  The Top 8 Win-OSX SBT to SRTS Software</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/new-expert-advice-for-efficiently-creating-srt-files/"><u>[New] Expert Advice for Efficiently Creating SRT Files</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/new-funimate-pro-unboxed-your-essential-apk-guide/"><u>[New] Funimate Pro Unboxed  Your Essential APK Guide</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/new-funimate-simplified-your-compreayer-guide/"><u>[New] Funimate Simplified  Your Compreayer Guide</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/new-innovative-approaches-to-healthcare-marketing-on-facebook/"><u>[New] Innovative Approaches to Healthcare Marketing on Facebook</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/new-innovative-approaches-to-producing-impressive-audio-teasers/"><u>[New] Innovative Approaches to Producing Impressive Audio Teasers</u></a></li>
<li><a href="https://extra-skills.techidaily.com/new-mastering-the-moment-best-drone-footage-editing-tools-ranked/"><u>[New] Mastering the Moment  Best Drone Footage Editing Tools Ranked</u></a></li>
<li><a href="https://instagram-video-files.techidaily.com/new-mastering-virality-in-instagram-clips-for-2024/"><u>[New] Mastering Virality in Instagram Clips for 2024</u></a></li>
<li><a href="https://facebook-record-videos.techidaily.com/new-the-ultimate-checklist-for-youtube-rule-adherence/"><u>[New] The Ultimate Checklist for YouTube Rule Adherence</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/updated-fix-coffee-stain-distortions-on-iphones-in-a-flash-for-free/"><u>[Updated] Fix Coffee Stain Distortions on iPhones in a Flash, for Free</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/updated-fix-for-freezing-photo-booth-videos-that-disrupt-usage/"><u>[Updated] Fix for Freezing Photo Booth Videos That Disrupt Usage</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/updated-freed-images-public-domain-canvas/"><u>[Updated] Freed Images  Public Domain Canvas</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/updated-freedom-in-viewing-is-vlc-more-powerful-than-mpc/"><u>[Updated] Freedom in Viewing  Is VLC More Powerful Than MPC?</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/updated-gigglegridsguild-funnyframefactory/"><u>[Updated] GiggleGridsGuild  FunnyFrameFactory</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/updated-horizonhawk-reality-check/"><u>[Updated] HorizonHawk Reality Check</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/updated-how-to-whip-up-a-stunning-facebook-collage-post/"><u>[Updated] How to Whip Up a Stunning Facebook Collage Post</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/updated-how-to-write-compelling-podcast-narratives-and-examples-at-no-cost/"><u>[Updated] How to Write Compelling Podcast Narratives & Examples at No Cost</u></a></li>
<li><a href="https://tiktok-videos.techidaily.com/updated-unlock-more-views-with-these-tiktok-text-tools-of-2023/"><u>[Updated] Unlock More Views with These TikTok Text Tools of 2023</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/2024-approved-guide-to-fade-out-music-in-premiere-pro/"><u>2024 Approved  Guide To Fade Out Music In Premiere Pro</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/2024-approved-how-to-forge-an-impeccable-vr-self-representation/"><u>2024 Approved  How to Forge an Impeccable VR Self-Representation</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/2024-approved-how-to-free-rotate-and-merge-videos-on-android/"><u>2024 Approved  How to Free Rotate and Merge Videos on Android</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/2024-approved-how-to-use-leading-lines-in-photography-for-iphone-photos/"><u>2024 Approved  How to Use Leading Lines in Photography for iPhone Photos</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/2024-approved-incorporating-spiritual-sounds-on-cellphones/"><u>2024 Approved  Incorporating Spiritual Sounds on Cellphones</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/evaluating-the-boundaries-of-hero5-sessions-for-2024/"><u>Evaluating the Boundaries of Hero5 Sessions for 2024</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/expert-advice-downloading-editing-and-personalizing-whatsapp-tones-for-both-platforms-for-2024/"><u>Expert Advice  Downloading, Editing & Personalizing WhatsApp Tones for Both Platforms for 2024</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/gopro-deep-dive-side-by-side-specification-comparison-for-2024/"><u>GoPro Deep Dive  Side-by-Side Specification Comparison for 2024</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/guiding-the-gaze-leading-line-techniques-for-iphones-for-2024/"><u>Guiding the Gaze  Leading Line Techniques for iPhones for 2024</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/harmonizing-background-sounds-with-film-trailers-for-2024/"><u>Harmonizing Background Sounds with Film Trailers for 2024</u></a></li>
<li><a href="https://fox-that.techidaily.com/hot-iphoneipad-troubles-uncover-reasons-and-fixing-methods-easily/"><u>Hot iPhone/iPad Troubles: Uncover Reasons & Fixing Methods Easily</u></a></li>
<li><a href="https://fix-guide.techidaily.com/how-to-flash-dead-vivo-s17t-safely-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>How to Flash Dead Vivo S17t Safely | Dr.fone</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/how-to-halt-spotify-from-automatically-playing-podcasts-for-2024/"><u>How to Halt Spotify From Automatically Playing Podcasts for 2024</u></a></li>
<li><a href="https://location-social.techidaily.com/how-to-sharefake-location-on-whatsapp-for-oneplus-ace-2-drfone-by-drfone-virtual-android/"><u>How to Share/Fake Location on WhatsApp for OnePlus Ace 2 | Dr.fone</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/ideal-steadicams-to-enhance-dslr-video-production-quality-for-2024/"><u>Ideal Steadicams to Enhance DSLR Video Production Quality for 2024</u></a></li>
<li><a href="https://sim-unlock.techidaily.com/in-2024-android-unlock-code-sim-unlock-your-poco-m6-pro-5g-phone-and-remove-locked-screen-by-drfone-android/"><u>In 2024, Android Unlock Code Sim Unlock Your Poco M6 Pro 5G Phone and Remove Locked Screen</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/in-2024-fading-out-sounds-effectively-using-lumafusion/"><u>In 2024, Fading Out Sounds Effectively Using Lumafusion</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/in-2024-from-spoken-words-to-written-text-ppt-innovation-guide/"><u>In 2024, From Spoken Words to Written Text  PPT Innovation Guide</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/in-2024-from-standard-screen-to-vr-world-smartphone-conversion-guide/"><u>In 2024, From Standard Screen to VR World  Smartphone Conversion Guide</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/in-2024-guide-to-exporting-pinterest-videos-into-mp3-format/"><u>In 2024, Guide to Exporting Pinterest Videos Into MP3 Format</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/in-2024-guide-to-making-an-impression-with-your-apple-podcast-entry/"><u>In 2024, Guide to Making an Impression with Your Apple Podcast Entry</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/in-2024-how-do-you-get-sun-stone-evolutions-in-pokemon-for-tecno-camon-20-drfone-by-drfone-virtual-android/"><u>In 2024, How Do You Get Sun Stone Evolutions in Pokémon For Tecno Camon 20? | Dr.fone</u></a></li>
<li><a href="https://location-social.techidaily.com/in-2024-how-to-changefake-your-meizu-21-pro-location-on-viber-drfone-by-drfone-virtual-android/"><u>In 2024, How to Change/Fake Your Meizu 21 Pro Location on Viber | Dr.fone</u></a></li>
<li><a href="https://android-location-track.techidaily.com/in-2024-how-to-track-samsung-galaxy-z-flip-5-location-by-number-drfone-by-drfone-virtual-android/"><u>In 2024, How to Track Samsung Galaxy Z Flip 5 Location by Number | Dr.fone</u></a></li>
<li><a href="https://digital-screen-recording.techidaily.com/in-2024-privishield-shield-and-cam-cover/"><u>In 2024, PriviShield Shield & Cam Cover</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/in-2024-why-does-imovie-crop-my-videos/"><u>In 2024, Why Does iMovie Crop My Videos?</u></a></li>
<li><a href="https://facebook-video-share.techidaily.com/in-2024-youtube-playlist-building-step-by-step-expertise/"><u>In 2024, YouTube Playlist Building  Step-by-Step Expertise</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/in-depth-analysis-applying-luts-to-elevate-your-cinematography-for-2024/"><u>In-Depth Analysis  Applying LUTs to Elevate Your Cinematography for 2024</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/in-depth-examination-androids-photography-solution-lightroom-for-2024/"><u>In-Depth Examination  Android's Photography Solution, Lightroom for 2024</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/in-depth-examination-lg-bp350-screen-specifications-and-reviews-for-2024/"><u>In-Depth Examination  LG BP350 Screen Specifications and Reviews for 2024</u></a></li>
<li><a href="https://ai-video-apps.techidaily.com/new-2024-approved-best-8k-video-editing-software/"><u>New 2024 Approved Best 8K Video Editing Software</u></a></li>
<li><a href="https://ai-video-apps.techidaily.com/new-in-2024-free-m4a-editor-software-top-5-options/"><u>New In 2024, Free M4A Editor Software Top 5 Options</u></a></li>
<li><a href="https://desktop-recording.techidaily.com/sound-capture-device-audit-for-2024/"><u>Sound Capture Device Audit for 2024</u></a></li>
<li><a href="https://tech-renaissance.techidaily.com/step-by-step-how-to-access-and-enjoy-3d-movie-night-with-fandango-from-the-comfort-of-home/"><u>Step by Step: How to Access and Enjoy 3D Movie Night with Fandango From the Comfort of Home</u></a></li>
<li><a href="https://on-screen-recording.techidaily.com/top-picks-for-traditional-japanese-huts-in-mc-worlds-for-2024/"><u>Top Picks for Traditional Japanese Huts in MC Worlds for 2024</u></a></li>
<li><a href="https://fox-that.techidaily.com/unlock-effective-voice-typing-on-your-iphone-with-these-5-essential-troubleshooting-steps/"><u>Unlock Effective Voice Typing on Your iPhone with These 5 Essential Troubleshooting Steps</u></a></li>
</ul></div>
