
```
AMP:~ AA$
AMP:~ AA$ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
==> This script will install:
/usr/local/bin/brew
/usr/local/Library/...
/usr/local/share/man/man1/brew.1
==> The following directories will be made group writable:
/usr/local/.
/usr/local/bin
/usr/local/include
/usr/local/lib
/usr/local/lib/pkgconfig
/usr/local/share
/usr/local/share/man
/usr/local/share/man/man1
/usr/local/share/man/man5
/usr/local/share/info
==> The following directories will have their owner set to AA:
/usr/local/.
/usr/local/bin
/usr/local/include
/usr/local/lib
/usr/local/lib/pkgconfig
/usr/local/share
/usr/local/share/man
/usr/local/share/man/man1
/usr/local/share/man/man5
/usr/local/share/info
==> The following directories will have their group set to admin:
/usr/local/.
/usr/local/bin
/usr/local/include
/usr/local/lib
/usr/local/lib/pkgconfig
/usr/local/share
/usr/local/share/man
/usr/local/share/man/man1
/usr/local/share/man/man5
/usr/local/share/info

Press RETURN to continue or any other key to abort
==> /usr/bin/sudo /bin/chmod g+rwx /usr/local/. /usr/local/bin /usr/local/include /usr/local/lib /usr/local/lib/pkgconfig /usr/local/share /usr/local/share/man /usr/local/share/man/man1 /usr/local/share/man/man5 /usr/local/share/info

WARNING: Improper use of the sudo command could lead to data loss
or the deletion of important system files. Please double-check your
typing when using sudo. Type "man sudo" for more information.

To proceed, enter your password, or type Ctrl-C to abort.

Password:
==> /usr/bin/sudo /usr/sbin/chown AA /usr/local/. /usr/local/bin /usr/local/include /usr/local/lib /usr/local/lib/pkgconfig /usr/local/share /usr/local/share/man /usr/local/share/man/man1 /usr/local/share/man/man5 /usr/local/share/info
==> /usr/bin/sudo /usr/bin/chgrp admin /usr/local/. /usr/local/bin /usr/local/include /usr/local/lib /usr/local/lib/pkgconfig /usr/local/share /usr/local/share/man /usr/local/share/man/man1 /usr/local/share/man/man5 /usr/local/share/info
==> /usr/bin/sudo /bin/mkdir /Library/Caches/Homebrew
==> /usr/bin/sudo /bin/chmod g+rwx /Library/Caches/Homebrew
==> /usr/bin/sudo /usr/sbin/chown AA /Library/Caches/Homebrew
==> Downloading and installing Homebrew...
remote: Counting objects: 3892, done.
remote: Compressing objects: 100% (3736/3736), done.
remote: Total 3892 (delta 33), reused 2404 (delta 21), pack-reused 0
Receiving objects: 100% (3892/3892), 3.39 MiB | 6.31 MiB/s, done.
Resolving deltas: 100% (33/33), done.
From https://github.com/Homebrew/homebrew
 * [new branch]      master     -> origin/master
HEAD is now at f20234a sslscan: add 1.11.1 bottle.
==> Installation successful!
==> Next steps
Run `brew help` to get started
AMP:~ AA$
```



Warning After Installation


```

➜  ~  brew doctor
Please note that these warnings are just used to help the Homebrew maintainers
with debugging if you file an issue. If everything you use Homebrew for is
working fine: please don't worry and just ignore them. Thanks!

Warning: Some directories in /usr/local/share/man aren't writable.
This can happen if you "sudo make install" software that isn't managed
by Homebrew. If a brew tries to add locale information to one of these
directories, then the install will fail during the link step.

You should probably `sudo chown -R $(whoami)` them:
    /usr/local/share/man/mann

Warning: python is symlinked to python3
This will confuse build scripts and in general lead to subtle breakage.

Warning: "config" scripts exist outside your system or Homebrew directories.
`./configure` scripts often look for *-config scripts to determine if
software packages are installed, and what additional flags to use when
compiling and linking.

Having additional scripts in your path can confuse software installed via
Homebrew if the config script overrides a system or Homebrew provided
script of the same name. We found the following "config" scripts:
    /Users/AA/anaconda/bin/curl-config
    /Users/AA/anaconda/bin/freetype-config
    /Users/AA/anaconda/bin/glue-config
    /Users/AA/anaconda/bin/libpng-config
    /Users/AA/anaconda/bin/libpng16-config
    /Users/AA/anaconda/bin/python3-config
    /Users/AA/anaconda/bin/python3.5-config
    /Users/AA/anaconda/bin/python3.5m-config
    /Users/AA/anaconda/bin/xml2-config
    /Users/AA/anaconda/bin/xslt-config
    /Users/AA/Library/Enthought/Canopy_64bit/User/bin/freetype-config
    /Users/AA/Library/Enthought/Canopy_64bit/User/bin/libpng-config
    /Users/AA/Library/Enthought/Canopy_64bit/User/bin/libpng16-config
    /Users/AA/Library/Enthought/Canopy_64bit/User/bin/python-config
    /Users/AA/Library/Enthought/Canopy_64bit/User/bin/python2-config
    /Users/AA/Library/Enthought/Canopy_64bit/User/bin/python2.7-config
    /Users/AA/Library/Enthought/Canopy_64bit/User/bin/wx-config
    /Users/AA/Library/Enthought/Canopy_64bit/User/bin/xml2-config

Warning: Enthought Python was found in your PATH.
This can cause build problems, as this software installs its own
copies of iconv and libxml2 into directories that are picked up by
other build systems.

Warning: Unbrewed dylibs were found in /usr/local/lib.
If you didn't put them there on purpose they could cause problems when
building Homebrew formulae, and may need to be deleted.

Unexpected dylibs:
    /usr/local/lib/libtcl8.6.dylib
    /usr/local/lib/libtk8.6.dylib

Warning: Unbrewed header files were found in /usr/local/include.
If you didn't put them there on purpose they could cause problems when
building Homebrew formulae, and may need to be deleted.

Unexpected header files:
    /usr/local/include/fakemysql.h
    /usr/local/include/fakepq.h
    /usr/local/include/fakesql.h
    /usr/local/include/itcl.h
    /usr/local/include/itcl2TclOO.h
    /usr/local/include/itclDecls.h
    /usr/local/include/itclInt.h
    /usr/local/include/itclIntDecls.h
    /usr/local/include/itclMigrate2TclCore.h
    /usr/local/include/itclTclIntStubsFcn.h
    /usr/local/include/mysqlStubs.h
    /usr/local/include/odbcStubs.h
    /usr/local/include/pqStubs.h
    /usr/local/include/tcl.h
    /usr/local/include/tclDecls.h
    /usr/local/include/tclOO.h
    /usr/local/include/tclOODecls.h
    /usr/local/include/tclPlatDecls.h
    /usr/local/include/tclThread.h
    /usr/local/include/tclTomMath.h
    /usr/local/include/tclTomMathDecls.h
    /usr/local/include/tdbc.h
    /usr/local/include/tdbcDecls.h
    /usr/local/include/tdbcInt.h
    /usr/local/include/tk.h
    /usr/local/include/tkDecls.h
    /usr/local/include/tkPlatDecls.h

Warning: Unbrewed .pc files were found in /usr/local/lib/pkgconfig.
If you didn't put them there on purpose they could cause problems when
building Homebrew formulae, and may need to be deleted.

Unexpected .pc files:
    /usr/local/lib/pkgconfig/tcl.pc
    /usr/local/lib/pkgconfig/tk.pc

Warning: Unbrewed static libraries were found in /usr/local/lib.
If you didn't put them there on purpose they could cause problems when
building Homebrew formulae, and may need to be deleted.

Unexpected static libraries:
    /usr/local/lib/libtclstub8.6.a
    /usr/local/lib/libtkstub8.6.a
➜  ~  brew doctor
```

Bash completion

```
➜  ~  brew install bash-completion
==> Downloading https://homebrew.bintray.com/bottles/bash-completion-1.3.el_capitan.bottle.1.tar.gz
######################################################################## 100.0%
==> Pouring bash-completion-1.3.el_capitan.bottle.1.tar.gz
==> Caveats
Add the following lines to your ~/.bash_profile:
  if [ -f $(brew --prefix)/etc/bash_completion ]; then
    . $(brew --prefix)/etc/bash_completion
  fi

Homebrew's own bash completion script has been installed to
  /usr/local/etc/bash_completion.d

Bash completion has been installed to:
  /usr/local/etc/bash_completion.d
==> Summary
🍺  /usr/local/Cellar/bash-completion/1.3: 188 files, 1.1M
➜  ~


```
