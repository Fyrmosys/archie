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


## Pacman 

_`pacman` needs to be run as root, so either log in as root using `sudo -i` or use `sudo infront of every command`_

### Update mirrors and uprgrade packages
`pacman -Syu`

### Install `sl`
`pacman -S sl`

### Install git
`pacman -S git`

### Install arch linx development package for c and c++
`pacman -S base-devel`

## Yay

_Wrapper for the `pacman` package manager_

### Install `yay`

`git clone https://aur.archlinux.org/yay.git yay && cd yay`

`makepkg -si`