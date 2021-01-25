# Git 

## INTRODUCTION



In order to explain Git, we have to first explain various aspects of Version Control.

* Version Control : 

   Version Control is a system that allows you to revisit various versions of a file or set of files by recording changes.
   
there are three type of version control :
1. Local Version Control : A Local VCS entails one database on your hard disk that stores changes to files
1. Centralized Version Control :  This system entails a single server storing all changes and file versions, which can be accessed by various clients.
1. Distributed Version Control : allows for multiple mirrored repositories, programmers working in teams can collaborate with each other in various ways to complete a joint project, which enables the use of various simultaneous workflows 

## So the git is :

`Snapshots`

Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it. If the file has not changed, Git only stores a reference to the already-stored identical version of it.

`Local Operations`

Git mostly relies on local operations because most necessary information can be found in local resources. This allows for process expediency because a project’s history resides on the local disk, eliminating the need to fetch history information from the server, and allowing one to continue work on a project even when not online or on a VPN.

`Tracking Changes`

Every single change applied to any file or directory is tracked by Git. And, as the gatekeeper, Git will always detect file corruption or loss of information in transit.

`Loss of Data`

Git is set up to greatly minimize the possibility of irreversible damage to files, such as accidentally lost data. Git makes it extremely difficult for a snapshot of your file that is committed to be lost.

`States`

Files in Git can reside in three main states: committed, modified and staged.

`Committed`

Data is securely stored in a local database

`Modified`

File has been changed but not committed to the database

`Staged`



![img6](https://blog.udemy.com/wp-content/uploads/2015/08/image066.png)

# History of Git

Git traces its roots to the open source software project Linux kernel. Developers of this project began using a DVCS called BitKeeper in 2002. In 2005, many of these developers stopped using this DVCS due to tension between the Linux kernel community and the company behind BitKeeper’s and the eventual revocation of the DVCS’ gratis status. Subsequently, Linus Torvalds, the chief architect of the Linux kernel, began creating Git. With the intention of creating a DVCS with a workflow design similar to that of BitKeeper, which was also fast, Git allowed for non-linear development via multiple branches, could support large projects, possessed strong mechanisms preventing corruption, and had a simple design. Since its inception in 2005, Git has become one of the most utilized Version Control Systems in the world.

Getting Started
Download Git
In order to use Git, your computer must have it available. If you already have Git on your computer, you should make sure you have the latest version.

Git can be installed in three ways:

Install as a package
Install via another installer
Download and compile the source code.
Mac OS X
Terminal

The simplest method for installing Git on a Mac (for Mavericks 10.9 and above) is running Git from the Terminal. If Git is not installed, you will see a prompt for installation.

Git Website

You can also download Git by visiting this link and following the posted directions:

http://git-scm.com/download/mac

GitHub

A third option is to install Git as part of the GitHub for Mac install. GitHub is repository hosting service, which we will discuss in a future section.

Download GitHub for Mac via the following link:

http://mac.github.com

Windows
Git Website

You can download Git by visiting this link and following the posted directions:

http://git-scm.com/download/win

GitHub

Install Git as part of the GitHub for Windows install.

http://windows.github.com

Linux
Package Manager

You can try installing Git via your distribution’s inherent package management tool.

For Fedora:

`$ sudo yum install git`
For Ubuntu:

`$ sudo apt-get install git`
Git Website

To download Git for Linux, visit this link and follow the posted directions:

http://git-scm.com/download/linux

Graphical Clients
Git includes inherent Graphical User Interface (GUI) tools. However, users can also utilize third-party tools created for particular platforms.

GUI Clients

You can access a variety of GUI clients for Mac, Windows, and Linux via the following link:

https://git-scm.com/downloads/guis


# **Congratulation!!** you learned new stuff 

you can share this infromation with your friends just copy this link !! https://mohdazzam.github.io/-reading-notes/read02b 

also you can go back to our Home page  [Markdown](https://mohdazzam.github.io/-reading-notes)
