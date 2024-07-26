# dotfiles

## TODO
 - Deprecate the old repo. 

## Basic Toolikit

```shell
sudo apt install kitty tmux vim neofetch btop
```
Clone the repo.

```shell
mkdir -p ~/src
cd ~/src
git clone git@github.com:lkarydas/dotfiles.git
```

Set symlinks.

```shell
ln -sf ~/src/dotfiles/.inputrc ~/.inputrc
ln -sf ~/src/dotfiles/.tmux.conf ~/.tmux.conf
# Kitty configuration.
curl -o ~/.config/kitty/mocha.conf https://raw.githubusercontent.com/catppuccin/kitty/main/themes/mocha.conf
ln -sf ~/src/dotfiles/kitty/kitty.conf ~/.config/kitty/kitty.conf
```

## Hyprland

```shell
ln -sf ~/src/dotfiles/hyprland/hyprland.conf ~/.config/hypr/hyprland.conf
```
