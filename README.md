**The power of [Blat](https://www.blat.net) with a user friendly GUI**

Special thanks goes to:
The user **guinness** from the **portablefreeware.com forums** - for helping to optimize the code for v1.3 and employ Blat's Unicode support. 

## Usage
All you have to do is launch **LWBlat GUI_x64.exe** or **LWBlat GUI_x32.exe** (see [difference](#what-is-the-difference-between-the-32-bit-and-the-64-bit-version)).

## System requirements
Windows 200X, Windows XP, Windows Vista, Windows 7-10

## Screenshots
### The menus

<img src="https://user-images.githubusercontent.com/1773306/236648017-b685bb3f-412c-46a8-93ce-666b303277d7.png" alt="Menu 1" width="30%">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="https://user-images.githubusercontent.com/1773306/90964683-82ab9b80-e4cb-11ea-9a84-685bfe79b235.png" alt="Menu 2" width="30%">

<img src="https://user-images.githubusercontent.com/1773306/90964691-8e975d80-e4cb-11ea-9727-5b8e265af1bd.png" alt="Menu 3" width="30%">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="https://user-images.githubusercontent.com/1773306/90964694-99ea8900-e4cb-11ea-8066-ab535fe47c0c.png" alt="Menu 4" width="30%">

### The Simulator
See [more info](#what-does-it-mean-a-simulator)

![Simulation mode](https://user-images.githubusercontent.com/1773306/236648078-94b232a1-9807-4c1f-9e89-5cf982c0f18b.png)

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
Because it's still a separate program which doesn't even have to be in the same folder. But if it's important for you, download [the PortableApps version](#what-is-the-portableapps-version).

#### Are the messages sent secured?
No, because Blat itself doesn't support it. It also means you can't use servers that don't support **insecure** sending. If you like to convince Blat makers to support it, please help asking [for OAuth support](https://sourceforge.net/p/blat/feature-requests/30/) and [for SSL support](https://sourceforge.net/p/blat/feature-requests/8/).

#### Can Blat even be used nowadays if most servers block insecure mode?
Not directly, because indeed most servers don't allow to use programs like Blat anymore. However, you can still use Blat as a simulator to try out every possible sending option. You can [convince here](https://sourceforge.net/p/blat/feature-requests/31/) Blat makers to add a direct simulation mode. Until then, that's why LWBlat GUI has a simulator (an embedded version of [LWSMTP-Server](https://github.com/lwcorp/lwsmtp-server), and of course external simulators can be used as well (like [Papercut SMTP](https://github.com/ChangemakerStudios/Papercut-SMTP)).

#### What does it mean a simulator?
As [this screenshot demonstrates](#the-simulator), it means you can play around with blat's various settings, then simulate how your message would have been received in someone's inbox. It's needed because of [Blat's inability to support modern public servers](https://github.com/lwcorp/lwblat/edit/main/README.md#are-the-messages-sent-secured).

### General

#### Is the program portable?
Yes, no installation is involved. You need to run the main program, see [usage](#usage).

#### What is the difference between the 32-bit and the 64-bit version?
There are no intentional differences. Even more so, the 32-bit version can still be used in 64-bit operating systems. But the 64-bit version is compiled specifically for such systems.

#### What is the PortableApps version?
While the program is [portable by design](#is-the-program-portable), this specific version is compatible with PortableApps ([see forum discussion](https://portableapps.com/node/26192)).

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
