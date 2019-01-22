# Setting up Freddy's mac

## Name it

- Select a _god_ name (like Osiris, Apollo, Isis, etc..).
- If no there are no _god_ names available, select an _Asymov_ novel name.
- If no there are no _Asymov_ names available, select a _Planet_ name.
- In the unlikely event that there were no _god_, _Asymov_, or planet name, choose a women name (like Isabella, Amy...). 

## Before setup

1. Encrypt the whole disk drive with filevault.
2. Register with appleid account.
3. Disable natural scrolling

#Installs

## Install tools

_use strap https://github.com/drfmunoz/strap_

###### Use zsh instead of bash

	chsh -s $(which zsh)

###### Oh-My-Zsh

Install [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)

	curl -L https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh | sh

###### Powerlines

Install the Inconsolata and other fonts  _(13/14pt)_
 
	git clone https://github.com/Lokaltog/powerline-fonts

Install [powerlines](https://github.com/Lokaltog/powerline) [OSX](https://powerline.readthedocs.io/en/latest/installation/osx.html#installation-osx)

	git clone https://github.com/Lokaltog/powerline
	cd powerline
	./setup.py build
	./setup.py install --user
	
###### Show all files

	defaults write com.apple.finder AppleShowAllFiles TRUE

###### Kill dashboard

	defaults write com.apple.dashboard mcx-disabled -boolean YES
	Killall Dock

## Install from Mac apple store

1. XCode	
2. Spark 
3. Keynote
4. Aperture
5. GoodNotes
6. Twitter
8. Kindle (use the retina [app](http://www.amazon.com/gp/feature.html/ref=kcp_mac_ln_ar?docId=1000464931))

## Install mac apps

# Post install

## Setup Mail, Dbx, Evnt, etc.

1. Setup Spark (gmail account).
2. Setup Aperture Library.
3. Sign into Dropbox (sync documents).
4. Sign into Evernote (sync notes).
5. Set zsh as the default shell (in iTerm).

## Setup Chrome
1. [Tab manager](https://chrome.google.com/webstore/detail/tab-manager/coonecdghnepgiblpccbbihiahajndda/related?hl=en)
2. [Grammarly](https://chrome.google.com/webstore/detail/grammarly-for-chrome/kbfnbcaeplbcioakkpcpgfkobkghlhen?hl=en)
3. [History search](https://chrome.google.com/webstore/detail/history-search/bojcckfnoicpmfgjhhoncpinbmechmkl?hl=en)
4. [Speed tracker](https://chrome.google.com/webstore/detail/speed-tracer-by-google/ognampngfcbddbfemdapefohjiobgbdl/related?hl=en)
5. [Momentum](https://chrome.google.com/webstore/detail/momentum/laookkfknpbbblfpciffpaejjkokdgca?hl=en)
6. [Bookmark search](https://chrome.google.com/webstore/detail/bookmark-search/hhmokalkpaiacdofbcddkogifepbaijk)
7. [Disable chrome notifications](http://productforums.google.com/forum/#!topic/chrome/oYp5lXA3dhg)
8. [1Password](https://chrome.google.com/webstore/detail/1password-extension-deskt/aomjjhallfgjeglblehebfpbcfeobpgk?hl=en)

## Name History

1. Trantor (2003-2005)
2. Isabella (2005 - 2007) -- ibook 12 inch
2. Osiris (2007 - 2010) -- macbook pro 15 inch (1st gen)
4. Seth (2010 - 2011) -- macbook pro 15 inch (unibody)
5. Apollo (2011 - 2013) -- macbook pro 13 inch (unibody)
6. Chronos (2013 - 2015) -- macbook pro retina 13 (unibody late 2012)
7. Mercury (2015 - present) -- Macbook pro retina 13 (unibody mid 2015)

# Unix

[Ctrl-z and ctrl-c](http://superuser.com/questions/262942/whats-different-between-ctrlz-and-ctrlc-in-unix-command-line)
[Screen and tmux](http://www.dayid.org/os/notes/tm.html)
[sed](http://www.grymoire.com/unix/sed.html)

## OSX tips 
[select by columns](http://one-line-it.blogspot.fr/2013/01/mac-os-x-select-by-column.html)

#### Other setup guides and 
[Setup dev machine from zero](http://net.tutsplus.com/tutorials/tools-and-tips/setting-up-a-mac-dev-machine-from-zero-to-hero-with-dotfiles/)
[mac dev setup (rails)](https://github.com/nicolashery/mac-dev-setup)

#### MISC

	defaults write com.apple.dock persistent-apps -array-add '{"tile-type"="spacer-tile";}'; killall Dock
