# Guide4ME
## Ubuntu tricks
### Change apt server
`sudo sed -i 's/kr.archive.ubuntu.com/mirror.kakao.com/g' /etc/apt/sources.list`
### install Basic package
`sudo apt-get install -y bc bison build-essential ccache clang curl flex fontconfig g++-multilib gcc-multilib gir1.2-clutter-1.0 gir1.2-gtop-2.0 gir1.2-nm-1.0 git-core gnupg gperf imagemagick lib32ncurses5-dev lib32readline-dev lib32z1-dev libc6-dev-i386 libgl1-mesa-dev liblz4-tool libncurses5 libncurses5-dev libsdl1.2-dev libssl-dev libx11-dev libxml2 libxml2-utils libxml2-utils libxml2-utils lzop m4 make openjdk-8-jdk pngcrush python rsync schedtool squashfs-tools unzip unzip wget x11proto-core-dev xsltproc xsltproc zip zip zlib1g-dev zlib1g-dev zlib1g-dev:i386 zsh`
### install git-repo
`mkdir ~/bin`  
`PATH=~/bin:$PATH`  
`curl https://storage.googleapis.com/git-repo-downloads/repo > ~/bin/repo`  
`chmod a+x ~/bin/repo`  
`sed -i 's/\/usr\/bin\/env python/\/usr\/bin\/env python3/' bin/repo`
### install Google Chrome
`wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb`  
`sudo dpkg -i google-chrome-stable_current_amd64.deb`
### install CoreCtrl (AMD Radeon GPU tool)
`sudo add-apt-repository ppa:ernstp/mesarc`  
`sudo apt-get update`  
`sudo apt-get install corectrl`
### install Gnome shell system monitor extension
https://extensions.gnome.org/extension/120/system-monitor/  

### PulseAudio Sample rate 
`pulseaudio -k` kill pulseaudio  
`/etc/pulse/daemon.conf`  
`pulseaudio --restart`  
  
### Git Editor Change
`git config --global core.editor "vim"`  

### DDC/CI control monitor  
`sudo apt-get install ddcutil`  
`sudo ddcutil getvcp 10 --display N`  
`sudo ddcutil setvcp 10 $brightness --display N`  

## VS Code tricks
change Ctrl Tab function like chrome  
https://stackoverflow.com/questions/38957302/is-there-a-quick-change-tabs-function-in-visual-studio-code

## Android links
Google Android  
https://source.android.com/

LineageOS  
https://github.com/lineageOS

Paranoid Android
https://github.com/AOSPA

PixelExperience  
https://github.com/PixelExperience/

Resurrection Remix OS  
https://github.com/ResurrectionRemix

Code Aurora Android for MSM Project  
https://wiki.codeaurora.org/xwiki/bin/QAEP/

SKY VEGA DEV TEAM  
https://github.com/sky-vega-dev-team
