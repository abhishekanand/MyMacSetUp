My Mac Set Up
============

My Mac Setup OSX Yosemite

[**Abhishek's Dotfiles Detail**](https://github.com/aageek/dotfiles)
 
# **Software Detail **

## Install Software

The software selected is software that is "installed after my first Macbook Pro.
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
	
### Devtool
1. GitHub for Mac

### Utility
1.  Atom editor
2.  LightPaper
	
### Random

1.  AdwareMedic
2.  AppCleaner
3.  Thunderbird
4.  VLC
5.  CCleaner 
6.  Snagit 12




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

**To verify  ```gcc ```  is installed **

```
$ gcc --version
Configured with: --prefix=/Applications/Xcode.app/Contents/Developer/usr --with-gxx-include-dir=/usr/include/c++/4.2.1
Apple LLVM version 6.0 (clang-600.0.56) (based on LLVM 3.5svn)
Target: x86_64-apple-darwin14.0.0
Thread model: posix

```

------------------------------------------------------

#PATH changes #

```
$ date
Sun Dec 21 00:09:26 PST 2014
$ echo $PATH
/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin
```