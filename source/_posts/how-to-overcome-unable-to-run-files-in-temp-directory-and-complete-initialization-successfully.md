---
title: How to Overcome 'Unable to Run Files in Temp Directory' And Complete Initialization Successfully
date: 2024-08-22 15:51:14
updated: 2024-08-24 12:57:13
tags:
  - win11
  - win10
  - win7
categories:
  - driver
description: This Article Describes How to Overcome 'Unable to Run Files in Temp Directory' And Complete Initialization Successfully
excerpt: This Article Describes How to Overcome 'Unable to Run Files in Temp Directory' And Complete Initialization Successfully
thumbnail: https://thmb.techidaily.com/d24f731fb7d4e16e9e3dad20fbd83add26d8b00ef3415c454c76fbd282fafbfc.jpg
---

## How to Overcome 'Unable to Run Files in Temp Directory' And Complete Initialization Successfully

While you upgrade[Driver Easy](https://tools.techidaily.com/drivereasy/download/)to the newer version, if you meet error “ **Unable to execute file in the temporary directory. Setup aborted. Error 5: Access is denied**”, please understand the problem is not caused by Driver Easy software issues. It is caused by system issues or protection software issues. You may also encounter this issue when you install some other new software. Here you will find the solutions how to fix this issue.   
  
[![Driver Easy - Unable to Update](https://images.drivereasy.com/wp-content/uploads/2015/12/Driver-Easy-Unable-to-Update.jpg)](https://images.drivereasy.com/wp-content/uploads/2015/12/Driver-Easy-Unable-to-Update.jpg)   
  
You can try the solutions below and find the one that works for you.   
  
**Solution 1:**Run the file as Administrator:  
  
1\. Right-click on the installer file.  
2\. Choose**Run as Administrator**. Then the software may be installed successfully.   
  
**Solution 2:**The problem may be caused due to security right issues. Try the following steps:  
  
1\. Navigate to**C:\\Users\\\[Username\]\\AppData\\Local**.  
2\. Right click on the**Temp**folder. Choose**Properties**.   
  
[![2](https://images.drivereasy.com/wp-content/uploads/2015/12/23.png)](https://images.drivereasy.com/wp-content/uploads/2015/12/23.png)   
  
3\. Click the**Security**tab and click**Advanced**.   
  
[![3](https://images.drivereasy.com/wp-content/uploads/2015/12/34.png)](https://images.drivereasy.com/wp-content/uploads/2015/12/34.png)   
  
4\. On the**Permissions**tab you should see permissions that are there. 3 permissions below you will see: ‘**SYSTEM** ‘ with Full control which applies to ‘This folder, subfolders and files’‘**Administrators**‘ with Full control which applies to ‘This folder, subfolders and files’ ‘**Your** **Username**‘ with Full control which applies to ‘This folder, subfolders and files’ These all 3 permissions should be inherited from the**C:\\Users\\\[Username\]\\**folder. If you don’t have the ‘Include inheritable permissions from this object’s parent’ option ticked, click on**Change Permissions…**.   
  
[![1](https://images.drivereasy.com/wp-content/uploads/2015/12/13-500x380.png)](https://images.drivereasy.com/wp-content/uploads/2015/12/13.png)   
  
5.Tick the box next to ‘Include inheritable permissions from this object’s parent’. Then click**Apply**and**OK** buttons. Click**Continue**if there are any problems, then remove the permissions that aren’t inherited.   
  
[![5](https://images.drivereasy.com/wp-content/uploads/2015/12/53-500x378.png)](https://images.drivereasy.com/wp-content/uploads/2015/12/53.png)   
  
After you follow steps above, you should have the permissions to write to the directory and you won’t get those error messages any more.   
  
**Solution 3:** It may be HIPS (Host-based Intrusion Prevention System HIPS) causing this false positive. Try fully disabling your anti-virus, anti-spyware and firewall applications.

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
