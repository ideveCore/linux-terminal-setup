#  Linux terminal setup

## Install Vim, Neovim and Lunarvim

In this tutorial we will install Vim, Neovim and Lunarvim and configure the basic plugins for coding in the terminal.

**Fast installation and configuration!**

### Dependencies
#### Python-* - Default in linux distributions
#### Pip:
  ##### In Debian or derivatives:
  
	sudo apt install python3-pip
  ##### In Arch or derivatives:
  	pacman -S python-pip
   ##### In Fedora:
   
	sudo dnf install python3-pip
	
#### Nodejs-*
  ##### In Debian or derivatives:
  
  	curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash - &&\
	sudo apt-get install -y nodejs
##### In Arch or derivatives:

	sudo pacman -Sy nodejs npm

##### In Fedora:

	sudo dnf install nodejs
	 
#### Essential packages for build
  ##### in Debian or derivatives:
  
	sudo apt install build-essential
  
  ##### in Arch or derivatives:
  
	sudo pacman -Sy base-devel
	  
  ##### in Fedora:
  
	sudo dnf install make automake gcc gcc-c++ kernel-devel
	
#### Vim
 ##### in Debian or derivatives:
  
	sudo apt install vim
  
  ##### in Arch or derivatives:
  
	sudo pacman -Sy vim
	  
  ##### in Fedora:
  
	sudo dnf install vim

#### Neovim

**Attention! In Debian and Fedora derivates its recommends build from source code Neovim, in Arch is not necessary because contains the neovim package up-to-date.**
##### In Fedora and Debian or derivatives:
	git clone https://github.com/neovim/neovim.git
	make CMAKE_BUILD_TYPE=RelWithDebInfo
	sudo make install
	
##### In Arch or derivatives:

	sudo pacman -Sy neovim
	
#### Neovim plugin - Neovim from Scratch

	git clone https://github.com/ngscheurich/nvim-from-scratch ~/.config/nvim

#### Lunarvim
	LV_BRANCH='release-1.3/neovim-0.9' bash <(curl -s https://raw.githubusercontent.com/LunarVim/LunarVim/release-1.3/neovim-0.9/utils/installer/install.sh)
