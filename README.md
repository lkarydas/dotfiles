# dotfiles

It's 2023 so it's time I kept my dot files in a repo called `dotfiles`. I previously had them in a repo called `config_files`. This was lame.

First thing on the list now is to deprecate the old repo. We will do that before we submit anything useful to the new repo. The reason for the urgency is the underscore in the repo name. Not cool.


# Initial

Clone the repo and create symbolic links.

```shell
mkdir -p ~/src
cd ~/src
git clone git@github.com:lkarydas/dotfiles.git
ln -sf ~/src/dotfiles/.inputrc ~/.inputrc
ln -sf ~/src/dotfiles/hyprland/hyprland.conf ~/.config/hypr/hyprland.conf
ln -sf ~/src/dotfiles/.tmux.conf ~/.tmux.conf
# Kitty configuration.
curl -o ~/.config/kitty/mocha.conf https://raw.githubusercontent.com/catppuccin/kitty/main/themes/mocha.conf
ln -sf ~/src/dotfiles/kitty/kitty.conf ~/.config/kitty/kitty.conf
