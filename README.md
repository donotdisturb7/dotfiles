# dotfiles

my sway dotfiles

Repo location:

```sh
~/dotfiles
```

## Install

Install Git and Stow:

```sh
sudo pacman -S git stow
```

Clone:

```sh
cd ~
git clone git@github.com:donotdisturb7/dotfiles.git dotfiles
cd ~/dotfiles
```

Preview links:

```sh
stow --target="$HOME" --simulate --verbose .
```

Create links:

```sh
stow --target="$HOME" --verbose .
```

This links files from `~/dotfiles` into the normal places, like:

```sh
~/.config/sway -> ~/dotfiles/.config/sway
~/.config/waybar -> ~/dotfiles/.config/waybar
~/.tmux.conf -> ~/dotfiles/.tmux.conf
~/Scripts -> ~/dotfiles/Scripts
```

