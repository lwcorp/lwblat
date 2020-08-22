**The power of [Blat](https://www.blat.net) with a user friendly GUI**

Special thanks goes to:
The user **guinness** from the **portablefreeware.com forums** - for helping to optimize the code for v1.3 and employ Blat's Unicode support. 

## Table of Contents  
1. [Usage](#usage)
1. [System requirements](#system-requirements)
1. [Screenshots](#screenshots)
   1. [The menus](#the-menus)
   1. [Easy way to search for additional arguments](#easy-way-to-search-for-additional-arguments)
1. [FAQ](#faq)
   1. [Introduction](#introduction)
      1. [What is Blat?](#what-is-blat)
      1. [What is LWBlat GUI?](#what-is-lwblat-gui)
      1. [Does LWBlat GUI require Blat itself?](#does-lwblat-gui-require-blat-itself)
      1. [Does LWBlat GUI use Blat's DLL file?](#does-lwblat-gui-use-blats-dll-file)
      1. [Why don't you add Blat inside the package?](#why-dont-you-add-blat-inside-the-package)
   1. [General](#general)
      1. [Is the program portable?](#is-the-program-portable)
      1. [What is the difference between the 32-bit and the 64-bit version?](#what-is-the-difference-between-the-32-bit-and-the-64-bit-version)
      1. [What is the PortableApps version?](#what-is-the-portableapps-version)
   1. [Window Controls](#window-controls)
      1. [Mail](#mail)
         1. [Why can there only be one attachment?](#why-can-there-only-be-one-attachment)
         1. [How do I actually send?](#how-do-i-actually-send)
      1. [Options](#options)
         1. [What is Hostname?](#what-is-hostname)
         1. [Can I use more charsets?](#can-i-use-more-charsets)
         1. [Can you include charset X by default?](#can-you-include-charset-x-by-default)
      1. [Preferences](#preferences)
         1. [Should I enable absolute paths?](#should-i-enable-absolute-paths)

## Usage
All you have to do is launch **LWBlat GUI_x64.exe** or **LWBlat GUI_x32.exe** (see [difference](#what-is-the-difference-between-the-32-bit-and-the-64-bit-version)).

## System requirements
Windows 200X, Windows XP, Windows Vista, Windows 7-10

## Screenshots
### The menus

<img src="https://user-images.githubusercontent.com/1773306/90964671-5c85fb80-e4cb-11ea-83d3-ea8805b569a2.png" alt="Menu 1" width="30%">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="https://user-images.githubusercontent.com/1773306/90964683-82ab9b80-e4cb-11ea-9a84-685bfe79b235.png" alt="Menu 2" width="30%">

<img src="https://user-images.githubusercontent.com/1773306/90964691-8e975d80-e4cb-11ea-9727-5b8e265af1bd.png" alt="Menu 3" width="30%">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="https://user-images.githubusercontent.com/1773306/90964694-99ea8900-e4cb-11ea-8066-ab535fe47c0c.png" alt="Menu 4" width="30%">

### Easy way to search for additional arguments
(additional arguments can be used in Options)

<img src="https://user-images.githubusercontent.com/1773306/90964695-a53db480-e4cb-11ea-91f9-95c901a3e004.png" alt="Search arguments" width="30%">

## FAQ

### Introduction
#### What is Blat?
Blat is a command line e-mailer for Windows. It's portable, it's small and it pretty much has every sending option one could possibly want. Alas, this abandonware's lack of GUI left it in a very user unfriendly state. That is, until LWBlat GUI came along.

#### What is LWBlat GUI?
LWBlat GUI continues where Blat left off. It combines the power of Blat with a user friendly GUI.

#### Does LWBlat GUI require Blat itself?
Yes, it's a GUI frontend for Blat. The actual mailer is still Blat so be sure to download it too. Then either put LWBlat GUI in the same folder or define Blat's location in LWBlat GUI's preferences.

#### Does LWBlat GUI use Blat's DLL file?
Yes, the sending process is properly done through Blat's DLL file.

#### Why don't you add Blat inside the package?
Because it's still a separate program which doesn't even have to be in the same folder.

### General

#### Is the program portable?
Yes, no installation is involved. You need to run the main program, see [usage](#usage).

#### What is the difference between the 32-bit and the 64-bit version?
There are no intentional differences. Even more so, the 32-bit version can still be used in 64-bit operating systems. But the 64-bit version is compiled specifically for such systems.

#### What is the PortableApps version?
While the program is [portable by design](#is-the-program-portable), this specific version is compatible with PortableApps ([See discussion](#https://portableapps.com/node/26192)).

### Window Controls
#### Mail

##### Why can there only be one attachment?
Because Blat is usually used for specialized jobs. If you need a full scale mailer, there's no point using Blat. With that said, you can use LWBlat GUI's Options to manually supply extra attachments.

##### How do I actually send?
You need to click Create and then Send. The Create button would create a command line to be delivered to Blat. LWBlat GUI would try to make sure the command is technically valid. Once you click Send, LWBlat GUI would interpret Blat's numeric result code.

#### Options
##### What is Hostname?
If you leave this field alone, it would be your computer's name on your LAN. It is a required e-mail header. Blat is about the only mailer in the world that lets you anonymize it.

##### Can I use more charsets?
LWBlat GUI lists some basic charsets. The last item in the list lets you enter any additional charset you like. Your custom choice would be kept in your settings until you change to another charset.

##### Can you include charset X by default?
You can submit a feature request.

#### Preferences
##### Should I enable absolute paths?
Only if you want to store the command line and use it in other computers with a different folder structure.

Otherwise, every path setting can be a relative path and even use environmental variables. This makes LWBlat GUI even more portable.
