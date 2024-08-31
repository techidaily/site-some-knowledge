---
title: "Ace Your Linux Workflow: The Ultimate Guide to Effortless File Cloning and Permission Management!"
date: 2024-08-27 17:22:58
updated: 2024-08-29 12:13:38
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

 Now that we’ve reclaimed ownership of the files and directories, we can fix the permissions.

##  Cloning Permissions With chmod

 This is a process very similar to the one we used with chown, but we need to be a little more careful with the permissions.

 Setting the ownership is easy. All the files and directories are owned by the same user, so they all receive the same settings. But directories and executable files must have the x (execute) permission set for them. Regular files don’t need that permissions set. So we need to create several sets of permissions and apply them to the appropriate files. We can do this in three steps.

 We’ll use a regular file as the reference file first. This will set the permissions as though everything is a regular file. Then we’ll use a reference _executable_ file to set the permissions for any shell scripts. Finally, we’ll use chmod in the traditional way to set the execute permission for the directories.

 Our first step is to use the regular file as the reference file:

sudo chmod -R --reference=/home/dave/Downloads/existing.dat project

![Recursively copying and setting file permissions using chmod](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/06/6-1.png) 

 We can use ls to see what effect this has had.

sudo ls -hld project

    
                    sudo ls -hl project

![Checking the file permissions on a directory and on its contents with ls](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/06/7-1.png) 

 The permissions from the reference file (read and write for the owner and group, and read-only for others) have been replicated on all files and directories.

 We need to restore the execute permission on any scripts. We’ve got a reference script we can take the permissions from.

sudo chmod -R --reference=/home/dave/Downloads/existing.sh project/*.sh

![Redcursively setting the permissions for executable scripts using chmod](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/06/8.png) 

 We’re using a wildcard "\*" because it’ll cope with any script file in the entire directory tree, regardless of its name.

 We can see that the execute permission has been set on the "appveyor.sh" file.

sudo ls -hl project

![Using ls to verify the execute permission has been set on an executable script](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/06/9.png) 

 Restoring the execute permission on the directories involves a neat trick. We can’t use a wildcard because it’s liable to match files too. So what we do is use the _uppercase_ X permission flag. This means "set the executable bit only if the target is a file with the executable bit _already_ set, or it is a directory."

 We can use this because our executable scripts already have the executable bit set, and they’ll retain it. All the directories in the directory tree will have the executable bit set, too.

sudo chmod -R +X project

![Using chmod to recusively set the execute permission on directories and subdirectories](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/06/10.png) 

 We now have things back to a working state with the correct ownership, correct permissions, and directories that let you cd into them.

ls -hl project

![Using ls to verify the permissions on directories and files](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/06/11.png) 

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
