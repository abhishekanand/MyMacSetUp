My Mac Set Up
===================

My Mac Setup OSX Yosemite 


My Mac Software installation List 

* Google Chrome 
* Firefox
* AdwareMedic
* AppCleaner
* Evernote
* github for Mac
* Pocket
* slack
* Twitter
* Thunderbird
* VLC
* CCleaner (12/19/2014)
*    12/20/2014
* Xcode  -> Appstore
* Xcode Command Line Tool
* atom editor
* lightpaper





## Install Software

The software selected is software that is "tried and true" --- software I need after any fresh install. I often install other software not listed here, but is handled in a case-by-case basis.

### Install from App Store

* Xcode  (Version 6.1.1)
	

### Install from Third-Party Websites 

* Browsers
	* Chrome (installed via Cask)
	* [Firefox](https://www.mozilla.org/en-US/firefox/new/)

#### ------------ ####

* Xode
* Xcode Command Line Developer Tools

```
$ xcode-select --install
xcode-select: note: install requested for command line developer tools
```

![]
(https://raw.githubusercontent.com/aageek/MyMacSetUp/master/images/Xcode_CLI.jpg)

Git (came with Xcode)
------------------------------

```
$ git --version
git version 1.9.3 (Apple Git-50)

$ which git
/usr/bin/git
```
**Installed Github for Mac **

```
$ ls /usr/local/bin/
git-media	github
$ ls -all /usr/local/bi

lrwxr-xr-x  1 root  wheel   67 Dec 19 01:42 git-media -> /Applications/GitHub.app/Contents/Resources/git-media/bin/git-media
lrwxr-xr-x  1 root  wheel   50 Dec 19 01:42 github -> /Applications/GitHub.app/Contents/MacOS/github_cli

```

** To verify  ```gcc ```  is installed **

```
$ gcc --version
Configured with: --prefix=/Applications/Xcode.app/Contents/Developer/usr --with-gxx-include-dir=/usr/include/c++/4.2.1
Apple LLVM version 6.0 (clang-600.0.56) (based on LLVM 3.5svn)
Target: x86_64-apple-darwin14.0.0
Thread model: posix

```
 