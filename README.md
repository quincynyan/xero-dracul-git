# **PS: This is just a fork of XeroLinux's old deleted rice. The creator said this is very bloated, but this repo exists just on the purpose of archiving. 

All credits go to [@TechXero](https://github.com/TechXero) as I didn't write any of this. 

_________________

<ins>***==========================================================================***<ins>

_________________

# This is XeroLinux's Dracul Rice

-> Some notes before proceeding :

> Applying this rice will override all your settings. So make sure to create a backup of your system either via Snapper if using it, or TimeShift. Don't worry though, script will attempt to create a backup for you of your ~/.config folder before proceeding. Still better be safe than sorry.

-> Performance issues :

> This rice as with all rices is not recommended to be used on lower-end hardware. iGPUs and less than 4GB RAM will result in sluggish and sometimes laggy behaviour. It's all due to Latte-Dock it's a memory hog, especially when using it way I do in my rices (sometimes 3 latte panels one dock). You've been warned. If you still insist on installing on lower-end systems, don't come to me asking for help..

![XeroDracul](https://i.imgur.com/eDxIOhk.jpg)

# Requirement for *Other* Arch KDE Distros ...

First off, note that if you want to use on other Arch based distros with KDE than **XeroLinux** you will need to add my repo since most of the packages are only available there.

Open the file `/etc/pacman.conf` and add my repo below anywhere :

```
[xerolinux_repo]
SigLevel = Optional TrustAll
Server = https://xerolinux.github.io/$repo/$arch
```
Save the file, and refresh databases via `sudo pacman -Sy` then follow below step...

# Installation

Just clone this repository, run terminal inside directory and run installer will do the following steps :

`git clone https://github.com/quincynyan/xero-dracul-git.git && cd xero-dracul-git && ./install.sh`

- Create a cbackup of your ~/.config folders
- Download and install necessary packages if needed...
- Override your settings and files with this rice's.
- Install and apply my XeroNord Grub theme.
- Reboot system to get everything loaded...

# F.A.Q

> Q: Will this rice work on other distros Like Fedora or Debian based ?<br />
> A : If it's not **Arch-KDE** or **XeroLinux** then no. Sorry.
>
> Q : I am running *Pre-Customized* **Arch** Distro with *KDE* can I use your rice ?<br />
> A : Short answer, *might*. Long answer, too many variables, I don't guarantee success.
>
> Q : After applying this rice on **XeroLinux** nice ASCII in neofetch gone how to get it back ?<br />
> A : To get Xero ASCII in neofetch back just unhash line 114 in `config.conf` inside `/.config/neofetch/`

# Disclosure

> Use this at your own Risk ! I won't be held liable if you didn't follow above recommendations.... Always Backup.. If you don't and break your system it's on you !!!!
