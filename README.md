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
###### iTerm2 

1. Install [iterm2](http://www.iterm2.com/)
2. Install [solarized](http://ethanschoonover.com/solarized) for [iterm](https://github.com/altercation/solarized/tree/master/iterm2-colors-solarized)

###### Install Oracle Java

1. Install 1.8 [Oracle Java (JDK7)](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
3. check [JAVAHOME](http://java.dzone.com/articles/java-findingsetting) and import development certs if needed.

###### Dot config files

Get dot config files from here (.zshrc,.vimrc,tmux, etc.)

	curl https://raw.github.com/drfmunoz/mac-setup/master/dotFiles/.tmux.conf > ~/.tmux.conf
	curl https://raw.github.com/drfmunoz/mac-setup/master/dotFiles/.zshrc > ~/.zshrc
	curl https://raw.github.com/drfmunoz/mac-setup/master/dotFiles/.vimrc > ~/.vimrc
	curl https://raw.github.com/drfmunoz/mac-setup/master/dotFiles/.gitconfig > ~/.gitconfig
	curl https://raw.github.com/drfmunoz/mac-setup/master/dotFiles/.gitignore_global > ~/.gitignore_global

###### SSH config

Get ssh config directory from _lunar_ (usb stick) -- [other dotFiles](http://dotfiles.github.io/)

###### Use zsh instead of bash

	chsh -s $(which zsh)

###### Oh-My-Zsh

Install [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)

	curl -L https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh | sh

###### Powerlines

Install the Inconsolata and other fonts  _(13/14pt)_
 
	git clone https://github.com/Lokaltog/powerline-fonts

Install [powerlines](https://github.com/Lokaltog/powerline) [OSX](https://powerline.readthedocs.org/en/latest/installation/osx.html#installation-osx)

	git clone https://github.com/Lokaltog/powerline
	cd powerline
	./setup.py build
	./setup.py install --user
	
###### Install homebrew

	ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

###### Install tree

	brew install tree

###### Install maven

	brew install maven

###### Install pip and aws

	curl https://bootstrap.pypa.io/get-pip.py > get-pip.py
	sudo python get-pip.py
	sudo pip install awscli

###### Change greeting message

	sudo defaults write /Library/Preferences/com.apple.loginwindow LoginwindowText 'Welcome to HOSTNAME (Freddy s haven)'

###### Show all files

	defaults write com.apple.finder AppleShowAllFiles TRUE

###### Kill dashboard

	defaults write com.apple.dashboard mcx-disabled -boolean YES
	Killall Dock

## Install from Mac apple store

1. XCode	
2. Airmail 
3. Keynote
4. Aperture
5. Evernote
6. Twitter
7. Eggscellent
8. Kindle (use the retina [app](http://www.amazon.com/gp/feature.html/ref=kcp_mac_ln_ar?docId=1000464931))

## Install mac apps

### Free/ Open Source

1. [Transmission](http://www.transmissionbt.com/download/)
2. [Mouapp](http://mouapp.com/)
3. [Pycharm](http://www.jetbrains.com/pycharm/)
4. [vlc](http://www.videolan.org/vlc/)
5. [Google Chrome](www.google.com/chrome‎)
6. [Mozilla Firefox](www.mozilla.org/en-US/firefox)
7. ~~[Quicksilver](http://qsapp.com/download.php) or [alfred](http://www.alfredapp.com/)~~ this is a new spotlight functionality
8. [Dropbox](https://www.dropbox.com/downloading)
9. [Spotify](https://www.spotify.com/download/mac)
10. [Menumeter](http://www.ragingmenace.com/software/menumeters/#download) - [requires patch panel](http://member.ipmu.jp/yuji.tachikawa/MenuMetersElCapitan/) for El Capitan
11. [TextMate 2](https://github.com/textmate/textmate)
12. [Open Office](https://www.openoffice.org/download/index.html)
13. [Cyberduck](http://cyberduck.io)
14. [Adium](https://adium.im) 
15. [Disk Inventory X](http://www.derlien.com/)
16. [Onyx](http://www.titanium.free.fr/pgs2/english/onyx_tiger.html)
17. [Skype](http://www.skype.com/en/download-skype/skype-for-computer/)
18. [Tunnelblick](https://code.google.com/p/tunnelblick/)
19. [monolingual](http://monolingual.sourceforge.net) -- use once. 
20. [Unarchiver](http://wakaba.c3.cx/s/apps/unarchiver.html) 
21. [R](http://www.r-project.org/)

### Proprietary with license

1. [Parallels](http://www.parallels.com/downloads/desktop/) -- got license for version 9
2. [IntelliJIdea](http://www.jetbrains.com/idea/) -- got license for version 12
3. [Webstorm](http://confluence.jetbrains.com/display/WI/Previous+WebStorm+Releases) -- got license for version 5
4. [IDocuments](http://www.icyblaze.com/idocument/) -- look for a replacement
5. [Game Dev Tycoon](http://www.greenheartgames.com/app/game-dev-tycoon/)
6. [Things](http://culturedcode.com/things/) and TLC [launchd job](http://nathangrigg.net/2012/07/schedule-jobs-using-launchd/)
7. Office -- got license and binaries in _lunar_.

# Post install

## Setup Mail, Dbx, Evnt, etc.

1. Setup Airmail (gmail account).
2. Import Music library from the time capsule.
3. Setup Aperture Library.
4. Sign into Dropbox (sync documents).
5. Sign into Evernote (sync notes).
6. Set zsh as the default shell (in iTerm).

## Setup Chrome
1. [Tab manager](https://chrome.google.com/webstore/detail/tab-manager/coonecdghnepgiblpccbbihiahajndda/related?hl=en)
2. [Clean the junk](https://chrome.google.com/webstore/detail/clean-the-junk/)
3. [History search](https://chrome.google.com/webstore/detail/history-search/bojcckfnoicpmfgjhhoncpinbmechmkl?hl=en)
4. [Speed tracker](https://chrome.google.com/webstore/detail/speed-tracer-by-google/ognampngfcbddbfemdapefohjiobgbdl/related?hl=en)
5. [Screen capture](https://chrome.google.com/webstore/detail/screen-capture-by-google/cpngackimfmofbokmjmljamhdncknpmg/related?hl=en)
6. [Bookmark search](https://chrome.google.com/webstore/detail/bookmark-search/hhmokalkpaiacdofbcddkogifepbaijk)
7. [Disable chrome notifications](http://productforums.google.com/forum/#!topic/chrome/oYp5lXA3dhg)

[Search engines backup restore](http://blog.ndrix.com/2010/10/sync-google-chrome-search-engines.html) _available on lunar_

### Setup IntellijIDEA

Install the [Solarized Theme](https://github.com/jkaving/intellij-colors-solarized)

### Add the cleanup launchd jobs

[scheduled jobs OSX](http://paul.annesley.cc/2012/09/mac-os-x-launchd-is-cool/)

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

#### OSX automation

[boxen](https://github.com/blog/1345-introducing-boxen)

#### MISC

	defaults write com.apple.dock persistent-apps -array-add '{"tile-type"="spacer-tile";}'; killall Dock
