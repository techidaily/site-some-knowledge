---
title: "Ace Your Linux Workflow: The Ultimate Guide to Effortless File Cloning and Permission Management!"
date: 2024-08-30T09:04:52.138Z
updated: 2024-08-31T09:04:52.138Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://thmb.techidaily.com/dae0a2870112b9a4ab1d756c066c8118fc25545f432e94a76fa542274edb47a5.jpg
---

## Ace Your Linux Workflow: The Ultimate Guide to Effortless File Cloning and Permission Management!

### Quick Links

* [The Mess and Stress of Bad Permissions](https://tech-haven.techidaily.com/leveraging-folders-for-coherent-gpt-3-discussions/)
* [The Problem?](https://tiktok-videos.techidaily.com/updated-innovative-techniques-for-self-duplication-on-social-medias-star-platform-tiktok/)
* [Cloning Ownership With chown](https://facebook-video-share.techidaily.com/optimizing-your-content-aspect-ratios-explained-for-youtube-users-for-2024/)
* [Cloning Permissions With chmod](https://on-screen-recording.techidaily.com/2024-approved-unveiling-the-top-methods-of-video-and-screenshots/)
* [Cloning Everything With setfacl](https://network-issues.techidaily.com/heal-visual-drifting-effects/)
* [Out of Chaos, Order](https://screen-video-capture.techidaily.com/updated-perfect-mac-imagery-a-guide-to-5-effective-snapshot-techniques-for-2024/)

### Key Takeaways

* Linux file permissions are crucial for control, and cloning correctly configured file settings can quickly fix messed-up permissions.
* Simple mistakes with chown and chmod commands can cause chaos, but chown and chmod cloning can efficiently restore file permissions.
* You can use the same cloning technique with Access Control Lists, too.

 Linux file permissions control who can do what with files and directories. But if they get messed up, restoring them can be a nightmare. Cloning a working file’s permissions is the fastest solution.

<!-- affiliate ads begin -->
<a href="https://mindmanager.sjv.io/c/5597632/1787667/20231" target="_top" id="1787667"><img src="//a.impactradius-go.com/display-ad/20231-1787667" border="0" alt="" width="728" height="90"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1787667/20231" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
##  The Mess and Stress of Bad Permissions

 On Linux, files and directories have a set of _permissions_. They control which actions can be performed, and by whom.

 Permissions either allow or deny someone reading from a file, writing to it, or executing it. For a file, executing means running a script or application. For a directory, execute means changing into that directory with [the cd command](https://audio-shaping.techidaily.com/updated-decoding-vimeos-video-dimensions-a-complete-perspective-on-aspect-ratios-for-2024/).

 Permissions directly affect the proper operation and security of your computer. Badly set permissions can cause havoc, effectively putting your data out of your reach.

 Files also have _owners_. New users, when created, are added to a group with the same name as their user login name. By default, a user owns all the files created by them, and the file’s group is set to the user’s group. A file or directory has three sets of permissions. One for the owner, another for members of the file's group, and a third for everyone not in the first two categories.

 Unpacking old archive files or restoring information from backups made on different computers can leave you with the files, but woefully inaccurate permissions. You can get into a similar situation if you make mistakes with the [chown](https://tech-recovery.techidaily.com/cant-remove-printer-on-windows-solved/) and [chmod](https://extra-guidance.techidaily.com/new-perfect-synchronization-enhancing-audio-visual-with-subtitles-in-wmp/) commands. The chmod command sets file permissions, and the chown command sets file ownership.

 Hand-fixing these types of error conditions is tedious. The answer is to use chown and chmod to clone the settings of a correctly configured file.

##  The Problem?

 I needed some files from an archive file I’d been sent. I [unpacked the archive](https://youtube-help.techidaily.com/first-steps-launching-a-youtube-channel-for-profit-for-2024/), but the extracted directory had a padlock badge on its icon.

![A directory icon with a padlock badge on it indicating the current user has no access to it](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/06/1-11.png) 

 I had to provide the root password to enter the directory. Double-clicking on its own wasn’t enough.

![GNOME asking for the root password to allow access to a directory](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/06/1a.png) 

 Checking with ls (again, using sudo) reveals the problem.

sudo ls -hld project

![Examing the permissions on a directory with ls](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/06/2-11.png) 

 The root user owns the directory, and nobody has read or write permissions.

 The files and subdirectories are also owned by root, and the permissions are a mishmash of different incorrect settings.

sudo ls -hl project

![Using ls to examine the permissions on files and subdirectories](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/06/3-9.png) 

 Let’s sort out the ownership issues first.

##  Cloning Ownership With chown

 I want to set the ownership of the file to me. My username is dave. We’ll use the chown command, and copy the ownership settings from a directory that is set correctly.

sudo chown -R --reference=/home/dave/Downloads project

![Recursively copying file ownership from one directory to another](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/06/4-3.png) 

 The **\--reference** option tells chown which directory to copy the permission settings from. The **\-R** (recursive) option tells chown to set the new permissions on the target directory, and on all files and subdirectories.

 We can check with ls that user dave is now the owner of the files and directories. We still need to use sudo because we haven’t sorted out the permissions yet.

sudo ls -hl project

![Checking the ownership of directories and files with ls](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/06/5-1.png) 

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4709458&QTY=1&AFFILIATE=108875&CART=1"><img src="https://3d-kstudio.com/wp-content/uploads/2019/10/Project-Manager-version-3-1600x900-768x419.jpg" border="0">Project Manager - Asset Browser for 3Ds Max</a>
<!-- affiliate ads end -->
 Now that we’ve reclaimed ownership of the files and directories, we can fix the permissions.

<!-- affiliate ads begin -->
<a href="https://purchase.swifdoo.com/order/checkout.php?PRODS=40002162&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/8b932759a5a04ddb34bf79e3f9072e4b/products/1_Product%20box%20white-1024x1024.png" border="0">SwifDoo PDF Perpetual (1 PC) Free upgrade. No monthly fees ever. 
</a>
<!-- affiliate ads end -->
##  Cloning Permissions With chmod

 This is a process very similar to the one we used with chown, but we need to be a little more careful with the permissions.

 Setting the ownership is easy. All the files and directories are owned by the same user, so they all receive the same settings. But directories and executable files must have the x (execute) permission set for them. Regular files don’t need that permissions set. So we need to create several sets of permissions and apply them to the appropriate files. We can do this in three steps.

 We’ll use a regular file as the reference file first. This will set the permissions as though everything is a regular file. Then we’ll use a reference _executable_ file to set the permissions for any shell scripts. Finally, we’ll use chmod in the traditional way to set the execute permission for the directories.

 Our first step is to use the regular file as the reference file:

sudo chmod -R --reference=/home/dave/Downloads/existing.dat project

![Recursively copying and setting file permissions using chmod](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/06/6-1.png) 

<!-- affiliate ads begin -->
<a href="https://unicoeye.pxf.io/c/5597632/2084396/18498" target="_top" id="2084396"><img src="//a.impactradius-go.com/display-ad/18498-2084396" border="0" alt="" width="1920" height="700"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2084396/18498" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 We can use ls to see what effect this has had.

sudo ls -hld project

    
                    sudo ls -hl project

![Checking the file permissions on a directory and on its contents with ls](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/06/7-1.png) 

<!-- affiliate ads begin -->
<span id="1997795">
					<video width="250" height="250" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1997795.jpeg"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/23621-1997795">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1997795.jpeg" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:250px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fproteahair.pxf.io%2Fc%2F5597632%2F1997795%2F23621'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1997795/23621" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 The permissions from the reference file (read and write for the owner and group, and read-only for others) have been replicated on all files and directories.

 We need to restore the execute permission on any scripts. We’ve got a reference script we can take the permissions from.

sudo chmod -R --reference=/home/dave/Downloads/existing.sh project/*.sh

![Redcursively setting the permissions for executable scripts using chmod](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/06/8.png) 

<!-- affiliate ads begin -->
<a href="https://ukaidot.sjv.io/c/5597632/1793237/19578" target="_top" id="1793237"><img src="//a.impactradius-go.com/display-ad/19578-1793237" border="0" alt="" width="1200" height="1200"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1793237/19578" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 We’re using a wildcard "\*" because it’ll cope with any script file in the entire directory tree, regardless of its name.

 We can see that the execute permission has been set on the "appveyor.sh" file.

sudo ls -hl project

![Using ls to verify the execute permission has been set on an executable script](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/06/9.png) 

 Restoring the execute permission on the directories involves a neat trick. We can’t use a wildcard because it’s liable to match files too. So what we do is use the _uppercase_ X permission flag. This means "set the executable bit only if the target is a file with the executable bit _already_ set, or it is a directory."

 We can use this because our executable scripts already have the executable bit set, and they’ll retain it. All the directories in the directory tree will have the executable bit set, too.

sudo chmod -R +X project

![Using chmod to recusively set the execute permission on directories and subdirectories](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/06/10.png) 

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=38729081&QTY=1&AFFILIATE=108875&CART=1"><img src="https://website-prod.cache.wpscdn.com/img/wps-spreadsheet-free-excel-editor-online-offline-1x.93e269d.png" border="0">
WPS Office Premium ( File Recovery, Photo Scanning, Convert PDF)--Yearly</a>
<!-- affiliate ads end -->
 We now have things back to a working state with the correct ownership, correct permissions, and directories that let you cd into them.

ls -hl project

![Using ls to verify the permissions on directories and files](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/06/11.png) 

<!-- affiliate ads begin -->
<a href="https://checkout.abbyy.com/order/checkout.php?PRODS=39254762&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/0e5fb5c76fca16adbee503c9aff393cd/products/11_FR-Badges-NEW-FR-Standard-16-WIN-200.png" border="0"> PDF application, powered by AI-based OCR, for unified workflows with both digital and scanned documents. </a>
<!-- affiliate ads end -->
<!-- affiliate ads begin -->
<a href="https://sentrypc.7eer.net/c/5597632/398457/3022" target="_top" id="398457"><img src="//a.impactradius-go.com/display-ad/3022-398457" border="0" alt="www.sentrypc.com" width="980" height="120"/></a><img height="0" width="0" src="https://sentrypc.7eer.net/i/5597632/398457/3022" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
##  Cloning Everything With setfacl

 If you’re using [Access Control Lists](https://video-capture.techidaily.com/new-2024-approved-ranking-the-top-5-instant-frame-recorder-apps/) (ACLs), you can still clone the settings from a correctly set file to other files. ACLs give you granular control, allowing you to do things like specify permissions on a per-user basis, with different users having different permissions.

 To clone the settings, we need to pipe the settings from our correctly configured file to the command to set the permissions.

 We can see the ACL settings on the existing file using the getfacl command.

getfacl existing.file

![Using getfacl to examine the ACL settings of a file](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/06/12.png) 

 The owner, dave has read, write, and execute permissions. User mary has read and write permissions. To clone these settings to the files in the project directory, we use the setfacl command. We pipe in the output from the getfacl command to make sure we get the ACL settings that we want. The files we want to apply the ACL settings to are in a directory called “source.”

getfacl /home/dave/Downloads/existing.file | setfacl --set-file=- source

![Piping the output of getfacl into setfacl to recusively copy ACL settings to files and directories](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/06/13.png) 

 The **\--set-file** option usually takes the name of a file that you want to copy the settings _from_. Using a single hyphen “-” as the filename tells setfacl to use stdin as its data source. This will be our piped data.

 Looking at any of the files in the source directory verifies that the copied ACL settings have been applied.

getfacl terminal.c

![Using getfacl to verify the ACL settings have been copied to another file](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/06/14.png) 

<!-- affiliate ads begin -->
<a href="https://tinyland.pxf.io/c/5597632/1793214/19135" target="_top" id="1793214"><img src="//a.impactradius-go.com/display-ad/19135-1793214" border="0" alt="" width="900" height="900"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1793214/19135" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
##  Out of Chaos, Order

 Seeing the mess you’re sometimes dumped into after downloading, restoring, or unarchiving files can make your heart sink. But it is easy enough to bring order to the chaos with just a few commands, used in the right order.

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


