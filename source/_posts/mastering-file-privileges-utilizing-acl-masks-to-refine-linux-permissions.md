---
title: "Mastering File Privileges: Utilizing ACL Masks to Refine Linux Permissions"
date: 2024-08-30T09:04:09.618Z
updated: 2024-08-31T09:04:09.618Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://thmb.techidaily.com/c6fb0c53f67d408b9f1a8e71dd93d74b8d8f511c12090374117c9c8e1782192a.jpg
---

## Mastering File Privileges: Utilizing ACL Masks to Refine Linux Permissions

### Quick Links

* [What Are ACL Masks?](https://ios-pokemon-go.techidaily.com/reasons-why-pokemon-gps-does-not-work-on-apple-iphone-xs-drfone-by-drfone-virtual-ios/)
* [Effective Permissions](https://location-social.techidaily.com/how-to-change-realme-12-pro-5g-location-on-skout-drfone-by-drfone-virtual-android/)
* [Default Masks](https://desktop-recording.techidaily.com/new-2024-approved-the-ultimate-list-best-mac-compatible-recorders/)

### Key Takeaways

* Access Control List (ACL) masks ensure compatibility with programs that aren't ACL-aware, translating ACL entries into POSIX permissions.
* ACL masks represent the maximum allowed permissions for any user or group object that isn't the owning user, group, or "other" class.
* When adding new ACL entries, the mask automatically adjusts to reflect the maximum permissions allowed for all named users or groups.

 Are you using [Access Control Lists (ACLs)](https://www.howtogeek.com/how-to-use-filesystem-acl-on-linux/) but are confused about the concept of masks? You're not alone. Let's dive into this important concept by taking a look at what they are and how they interact with Linux file system permissions.

<!-- affiliate ads begin -->
<a href="https://otszone.ots7.com/order/checkout.php?PRODS=4713322&QTY=1&AFFILIATE=108875&CART=1"><img src="https://green.ots7.com/screenshots/OtsAV/OtsAVRadio1.90-300x188.jpg" border="0">OtsAV Radio Webcaster</a>
<!-- affiliate ads end -->
##  What Are ACL Masks?

 ACL masks are a way to ensure permissions interoperability with programs and utilities that aren't ACL-aware.

 An ACL mask on a file or directory equates to the _maximum_ permissions allowed to any user or group object that isn't the owning user, group, or "other" class of the [user/group/other class paradigm](https://ai-driven-video-production.techidaily.com/new-add-motion-to-your-messages-top-text-animation-apps-for-phones-for-2024/). To put it another way, it _translates_ ACL entries into POSIX permissions for the sake of backward compatibility.

 Let's take a look at a newly created file we'll be working with in this article, mysupersecretfile.txt:

        `ls -l mysupersecretfile.txt`
    
![A terminal window showing the ls command and its output.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/1-20.png) 

 Pretty straightforward permissions for such a sensitive document, right?

 Notice the dot (.) after the permissions set. This indicates an SELinux context, which is unrelated to ACLs or ACL masks.

 For clarity, let's also examine the ACL entries for the file, using the getfacl command:

        `getfacl mysupersecretfile.txt`
    
![A terminal window showing the getfacl command and its output, with minimal ACL permissions.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/2-20.png) 

<!-- affiliate ads begin -->
<a href="https://estore.zonealarm.com/order/checkout.php?PRODS=38658749&QTY=1&AFFILIATE=108875&CART=1"><img src="https://sc1.checkpoint.com/sc1/za/images/boxes/pa_500.png" border="0">ZoneAlarm Pro Antivirus + Firewall NextGen</a>
<!-- affiliate ads end -->
 The current ACL entries for owning user and group entries map directly to the actual POSIX owning user and owning group of the file. This is normal for any file that doesn't have extended ACL entries, and is called "minimal ACLs".

 Let's say we received a request to add a user called manager as an ACL entry to this file, with read permissions. We'll accomplish this with the setfacl command. Then, let's examine the new ACL permissions using the ls and getfacl commands:

        `setfacl -m u:manager:r mysupersecretfile.txt  
ls -l mysupersecretfile.txt  
getfacl mysupersecretfile.txt`
    
![A terminal window showing the setfacl command to add a user ACL entry, the ls -l command, and the getfacl command and their outputs reflecting the new permissions.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/3-20.png) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2082535/7443" target="_top" id="2082535"><img src="//a.impactradius-go.com/display-ad/7443-2082535" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2082535/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 You'll now notice the "+" sign alongside the permissions entries in the ls command, indicating that there are ACL entries associated with the file.

 Do you see the **mask** line in the output of the getfacl command now? In addition to the manager user's extended ACL entry, this mask entry has been automatically assigned. This is necessary; it represents the maximum permissions allowed for any named user or group object (again, besides the owner user and owning group objects). Right now, the read permission equates to the read permission of the existing mask.

 Now let's add another user from a second request, contractor, to the ACL of our file. This time, however, we need to give them read and write permissions. Let's see how that affects the mask:

        `setfacl -m u:contractor:rw mysupersecretfile.txt  
getfacl mysupersecretfile.txt`
    
![A terminal window showing the setfacl command to add the contractor user with read and write permissions, and getfacl command and its output, particularly the modified mask permissions..](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/4-16.png) 

<!-- affiliate ads begin -->
<a href="https://store.bitdefender.com/affiliate.php?ACCOUNT=BITLATIN&AFFILIATE=108875&PATH=http%3A%2F%2Fwww.bitdefender.com%2Fbusiness%3FAFFILIATE%3D108875%26RESOURCE%3D30%2525%2BOff%2Ball%2BGravityZone%2BProducts"><img src="https://www.bitdefender.com/content/dam/bitdefender/business/campaign/1200X628.png" border="0"></a>
<!-- affiliate ads end -->
 Now, in addition to the manager (r) ACL entry, we also see the contractor (rw) entry. But why did the mask entry change to read and write?

 When we added the contractor user with read and write permissions, it affected the ACL mask because, as I mentioned above, the mask relates to the _maximum_ allowed permissions of ACL users and group entries. Since we added write permissions to the contractor user's ACL entry, the mask also gets the write permission.

 When working with ACLs, you'll see that the role of the group class permissions (such as with the output of the **ls -l** command) is re-purposed to reflect the ACL mask. Don't worry though, the group owner permissions are still reflected as the 'owning group' ACL entry.

 Keep in mind that if you add another user with fewer permissions, for example read-only, they do not inherit the mask permissions—just like the manager user didn't get the write permission when we added the contractor user's ACL entry.

<!-- affiliate ads begin -->
<a href="https://caperobbin.sjv.io/c/5597632/2006118/18460" target="_top" id="2006118"><img src="//a.impactradius-go.com/display-ad/18460-2006118" border="0" alt="" width="300" height="250"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2006118/18460" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
##  Effective Permissions

 We can set the mask entry permissions manually by using the setfacl command. This will allow us to filter any named user and/or group permissions set on the file at the same time, or for existing users' ACL entries of the file, to the lowest common denominator. This is called effective permissions.

 Let's set the mask on our file to read-only, and then take a fresh look at the ACL entries:

        `setfacl -m m::r mysupersecretfile.txt  
getfacl mysupersecretfile.txt  
`
    
![A terminal window showing the setfacl command, modifying the mask, and the getfacl command showing effective permissions.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/6-13.png) 

 The comment showing the contractor user's effective permissions lets us know that, even though they were granted read and write permissions, in reality, they only have read permission. Modifying the mask caused this. If we look at the file again with **ls -l**, we'll see the group class permissions (which again is re-purposed to reflect the mask) have changed:

        `ls -l mysupersecretfile.txt`
    
![A terminal window showing the ls command and its output with new group class permissions.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/7-14.png) 

<!-- affiliate ads begin -->
<a href="https://store.revouninstaller.com/order/checkout.php?PRODS=28010250&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/4282ec8de8c9be897e7aff4aa231b1a4/336__280a.jpg" border="0"></a>
<!-- affiliate ads end -->
 If you want to add a named user or group ACL entry, but don't want to recalculate the mask, you can use **\-n** alongside setfacl. This will restrict the ACL you're adding to the maximum permissions allowed by the mask (shown by the effective permissions of the entry). This isn't the default, though; keep in mind that the mask isn't a form of [mandatory access control](https://en.wikipedia.org/wiki/Mandatory%5Faccess%5Fcontrol). Let's try that below:

        `setfacl -n -m u:milton:rwx mysupersecretfile.txt  
getfacl mysupersecretfile.txt  
`
    
![A terminal window showing the setfacl command, adding rwx permissions for the milton user, and getfacl command showing effective permissions of r, due to the use of the -n parameter.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/8-12.png) 

##  Default Masks

 When you're working with ACLs, the concept of default masks is very similar to default ACL entries. For example, when you add a default mask to a directory, all newly created files and subdirectories inside of it will inherit that same mask (as well as the default mask entry). Just use the **\-d** parameter with the setfacl command to apply a default mask:

        `mkdir mysupersecretdirectory  
setfacl -d -m m::rX mysupersecretdirectory/  
getfacl mysupersecretdirectory/  
mkdir mysupersecretdirectory/mysupersecretsubdirectory/  
getfacl mysupersecretdirectory/mysupersecretsubdirectory/`
    
![A terminal window showing the mkdir, setfacl and getfacl commands to reflect a default mask assignment](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/9-7.png) 

 Default masks, and default ACL entries for that matter, are only applicable to directories since they're the only objects that can contain files and/or other directories inside of them to apply these inheritable entries to.

---

 ACL masks are a way to ensure the security of ACLs is handled properly, regardless of the capabilities of the program that's manipulating them.

 As technology, software, and security concepts continue to rapidly evolve, it's important to remember that backward compatibility is paramount for many of us, and must be honored alongside new advancements. Of course, that doesn't mean you can't have new bells and whistles, it just means that those new bells and whistles should adhere to existing standards.

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


