# arch-notes

_quick notes while learning arch_

## Environment

### Vagrant

Vagrant was used for local vm testing.

_after installing vagrant and virtualbox_

		vagrant init archlinux/archlinux
		vagrant up && vagrant ssh

_to kill it_

		vagrant halt && vagrant destroy -y


## Package Manager

### Pacman 

_`pacman` needs to be run as root, so either log in as root using `sudo -i` or use `sudo infront of every command`_

#### Update mirrors and uprgrade packages
`pacman -Syu`

#### Install `sl`
`pacman -S sl`

#### Install vim

`pacman -S neovim`

#### Install git
`pacman -S git`

#### Install arch linx development package for c and c++
`pacman -S base-devel`

### Yay

_Wrapper for the `pacman` package manager_

#### Install `yay`

`git clone https://aur.archlinux.org/yay.git yay && cd yay`

`makepkg -si`

## Alias and Function files

add `source ~/git/dots/jenniferannegarner.sh` to either `~/.bash_profile` or `~/.bashrc`

## Python

_need python for apps_

Just search for pyhton using yay...

_yay python_

### Pip

#### Install pip

`yay -S python-pip --noconfirm`

_check if installed_

`which pip`

#### Install virtualenv

_to keep things clean_

`pip install virtualenv --user`

_add to path_

`echo export PATH=$PATH:/home/vagrant/.local/bin >> ~/.bashrc`

##### Create virtual enviornment for python apps

_TODO : create a function for this, to switch on-demand_

`virtualenv venv`

_Add to .bashrc_

`echo source /home/vagrant/venv/bin/activate >> ~/.bashrc`

To exit use `deactivate`

#### Pyhton apps

`pip3 install jrnl`

`pip3 install awscli`