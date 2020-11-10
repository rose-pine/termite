![alt text](https://cdn.discordapp.com/attachments/608697372054126594/775783910243303504/unknown.png)

# Overview
In this repository you'll be able to use Rosé Pine color scheme in termite, how to install termite, load the config and keep going using termite.

# Termite Installation
AUR

``yay -S termite
``


From source


sudo apt update

sudo apt install build-essential

sudo apt-get install -y git g++ libgtk-3-dev gtk-doc-tools gnutls-bin valac intltool libpcre2-dev libglib3.0-cil-dev libgnutls28-dev libgirepository1.0-dev libxml2-utils gperf

git clone --recursive https://github.com/thestinger/termite.git
cd termite

make

sudo make install

sudo ldconfig

sudo mkdir -p /lib/terminfo/x

sudo ln -s /usr/local/share/terminfo/x/xterm-termite /lib/terminfo/x/xterm-termite

sudo update-alternatives --install /usr/bin/x-terminal-emulator x-terminal-emulator /usr/local/bin/termite 60

# Font
In order to use this config, you must have FiraCode Nerd Font, here's how to install it.

Install the .zip file called FiraCode Nerd Font from https://www.nerdfonts.com/font-downloads
mkdir ~/.local/share/fonts/

cp ~/Downloads/FiraCode.zip ~/.local/share/fonts/

cd ~/.local/share/fonts/

unzip FiraCode.zip

fc-cache -fv

# Cloning this repository 
`git clone https://github.com/rose-pine/termite.git
`

# Creating your termite config folder
`mkdir ~/.config/termite
`

# Making your termite follow this config
`
cp -r termite ~/.config/termite
`
# Final steps
After doing that, you're done, just save the changes and restart termite


