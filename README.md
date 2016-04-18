# .emacs.d
My personal emacs settings to optimize coding efficiency. 

## Setup
To get all the dependencies: 
```
git clone --recursive git://github.com/magnars/.emacs.d.git
```

###Installing on OS X: 
```
brew update
brew install emacs --cocoa
brew linkapps emacs
```
The last step is optional, but it’s recommended if you like to start Emacs from the launchpad or from Spotlight.

You can create an alias in your shell and when you invoke 'emacs' it will run the newly installed version:
```
$ alias emacs="/usr/local/Cellar/emacs/24.x/Emacs.app/Contents/MacOS/Emacs -nw"
```
To make it permanent, if using bash, add that line to ~/.bash_profile.


###Installing on Ubuntu 14.04: 
```
sudo apt-get install build-essential
sudo apt-get build-dep emacs24
wget http://ftp.gnu.org/gnu/emacs/emacs-24.5.tar.gz 
cd ~/Downloads && tar -xf emacs-24.5.tar.* && cd emacs-24.5
./configure
make
sudo make install
```
###Running on Chrome OS: 
Open a new terminal window
```
ctrl+alt+t
```
Access Shell 
```
$ shell
```
Launch in a new tab with Xiwi:
```
$ sudo enter-chroot xiwi -T emacs
```

