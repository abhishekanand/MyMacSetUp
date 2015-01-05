My Mac Set Up
============

My Mac Setup OSX Yosemite

[**Abhishek's Dotfiles Detail**](https://github.com/aageek/dotfiles)
 
# **Software Detail **

## Install Software

The software selected is software that is installed after my first Macbook Pro.
### Install from App Store

1.  Xcode  (Version 6.1.1)
2.  Alfred
3.  Evernote
4.  Pocket
5.  slack
6.  Twitter

## Install from Third-Party Websites

### Browsers
1. Chrome (installed via Cask)
2. [Firefox](https://www.mozilla.org/en-US/firefox/new/)
	
### Devtools
1. GitHub for Mac

### Utility Software
1.  Atom editor
2.  Brackets Editor
3.  [LightPaper](http://www.ashokgelal.com/lightpaper-for-mac/) - MarkDown Editor
4.  [Inky for Mac](http://inky.com/) - Email Client
5.  [Homebrew](http://brew.sh/)
6.  [Homebrew casks](http://caskroom.io/)
7.  iTerm 2
8.  oh-my-zsh 
	
### Randoms

1.  AdwareMedic
2.  AppCleaner
3.  Thunderbird
4.  VLC
5.  CCleaner 
6.  Snagit 12
7.  Spotify 
8.  Java 8 Update 25



#Installation #

* Xode
* Xcode Command Line Developer Tools

```
$ xcode-select --install
xcode-select: note: install requested for command line developer tools
```

![]
(https://raw.githubusercontent.com/aageek/MyMacSetUp/master/images/Xcode_CLI.jpg)

Git (version installed with Xcode)
------------------------------

```
$ git --version
git version 1.9.3 (Apple Git-50)

$ which git
/usr/bin/git
```
**Installed Github for Mac  (via GUI )**

```
$ ls /usr/local/bin/
git-media	github
$ ls -all /usr/local/bi

lrwxr-xr-x  1 root  wheel   67 Dec 19 01:42 git-media -> /Applications/GitHub.app/Contents/Resources/git-media/bin/git-media
lrwxr-xr-x  1 root  wheel   50 Dec 19 01:42 github -> /Applications/GitHub.app/Contents/MacOS/github_cli

```

**To verify  ```gcc ```  is installed**

```
$ gcc --version
Configured with: --prefix=/Applications/Xcode.app/Contents/Developer/usr --with-gxx-include-dir=/usr/include/c++/4.2.1
Apple LLVM version 6.0 (clang-600.0.56) (based on LLVM 3.5svn)
Target: x86_64-apple-darwin14.0.0
Thread model: posix

```

**Installation Homebrew**


```
$ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
==> This script will install:
/usr/local/bin/brew
/usr/local/Library/...
/usr/local/share/man/man1/brew.1
==> The following directories will be made group writable:
/usr/local/.
/usr/local/bin
==> The following directories will have their group set to admin:
/usr/local/.
/usr/local/bin

Press RETURN to continue or any other key to abort
==> /usr/bin/sudo /bin/chmod g+rwx /usr/local/. /usr/local/bin

WARNING: Improper use of the sudo command could lead to data loss
or the deletion of important system files. Please double-check your
typing when using sudo. Type "man sudo" for more information.

To proceed, enter your password, or type Ctrl-C to abort.

Password:
==> /usr/bin/sudo /usr/bin/chgrp admin /usr/local/. /usr/local/bin
==> /usr/bin/sudo /bin/mkdir /Library/Caches/Homebrew
==> /usr/bin/sudo /bin/chmod g+rwx /Library/Caches/Homebrew
==> Downloading and installing Homebrew...
remote: Counting objects: 223118, done.
remote: Compressing objects: 100% (58737/58737), done.
remote: Total 223118 (delta 163180), reused 223056 (delta 163134)
Receiving objects: 100% (223118/223118), 50.62 MiB | 2.71 MiB/s, done.
Resolving deltas: 100% (163180/163180), done.
From https://github.com/Homebrew/homebrew
 * [new branch]      master     -> origin/master
HEAD is now at 6d4fe18 Forward arguments in IRB formula helpers
==> Installation successful!
==> Next steps
Run `brew doctor` before you install anything
Run `brew help` to get started
$ brew doctor
Your system is ready to brew.
$ 

```

**Installation Homebrew casks**

```
$ brew install caskroom/cask/brew-cask
Cloning into '/usr/local/Library/Taps/caskroom/homebrew-cask'...
remote: Counting objects: 115028, done.
remote: Compressing objects: 100% (22/22), done.
remote: Total 115028 (delta 10), reused 0 (delta 0)
Receiving objects: 100% (115028/115028), 31.89 MiB | 1021.00 KiB/s, done.
Resolving deltas: 100% (75837/75837), done.
Checking connectivity... done.
Tapped 1 formula
==> Installing brew-cask from caskroom/homebrew-cask
==> Cloning https://github.com/caskroom/homebrew-cask.git
Cloning into '/Library/Caches/Homebrew/brew-cask--git'...
remote: Counting objects: 2611, done.
remote: Compressing objects: 100% (2339/2339), done.
remote: Total 2611 (delta 278), reused 777 (delta 258)
Receiving objects: 100% (2611/2611), 5.57 MiB | 1007.00 KiB/s, done.
Resolving deltas: 100% (278/278), done.
Checking connectivity... done.
Note: checking out '4e59f6c55b67ed078885c2ced58a75c9940b6e40'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by performing another checkout.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -b with the checkout command again. Example:

  git checkout -b new_branch_name

==> Checking out tag v0.52.0
==> Patching
🍺  /usr/local/Cellar/brew-cask/0.52.0: 2358 files, 9.3M, built in 10 seconds
$ 

```

**Installation oh-my-zsh**

```
$ curl -L http://install.ohmyz.sh | sh 
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   115  100   115    0     0    329      0 --:--:-- --:--:-- --:--:--   330
100  1906  100  1906    0     0   2708      0 --:--:-- --:--:-- --:--:--  5974
Cloning Oh My Zsh...
Cloning into '/Users/Anand/.oh-my-zsh'...
remote: Counting objects: 11504, done.
remote: Total 11504 (delta 0), reused 0 (delta 0)
Receiving objects: 100% (11504/11504), 2.10 MiB | 486.00 KiB/s, done.
Resolving deltas: 100% (6289/6289), done.
Checking connectivity... done.
Looking for an existing zsh config...
Using the Oh My Zsh template file and adding it to ~/.zshrc
Copying your current PATH and adding it to the end of ~/.zshrc for you.
Time to change your default shell to zsh!
Changing shell for Anand.
Password for Anand: 
         __                                     __   
  ____  / /_     ____ ___  __  __   ____  _____/ /_  
 / __ \/ __ \   / __ `__ \/ / / /  /_  / / ___/ __ \ 
/ /_/ / / / /  / / / / / / /_/ /    / /_(__  ) / / / 
\____/_/ /_/  /_/ /_/ /_/\__, /    /___/____/_/ /_/  
                        /____/                       ....is now installed!


 Please look over the ~/.zshrc file to select plugins, themes, and options.


 p.s. Follow us at http://twitter.com/ohmyzsh.


 p.p.s. Get stickers and t-shirts at http://shop.planetargon.com.
$ 

```
* NOTE : After installation of oh-my-zsh default shell for Terminal and iTerm 2 changed to zsh . I changed terminal shell  back to  bash and iTerm 2 to zsh.

 *Termimal  : Go to the Users & Groups pane of the System Preferences -> Select the User -> Click the lock to make changes (Bottom left corner) -> right click the Current user select Advanced options... -> Select the Login Shell: /bin/bash and OK*

*iTerm 2 : preferences Profiles Tab -> General section set Command to: /bin/zsh --login*

![]
(https://raw.githubusercontent.com/aageek/MyMacSetUp/master/images/zsh.jpg)

------------------------------------------------------

#PATH changes #

```
$ date
Sun Dec 21 00:09:26 PST 2014
$ echo $PATH
/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin
```