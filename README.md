# .dotfiles
My Linux configuration files.

Made for Arch Linux with KDE Plasma. Might break (things) on other setups.
## Installation
```
git clone --bare https://github.com/Armadillan/.dotfiles.git $HOME/.dotfiles
alias dotfiles='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'
dotfiles checkout
dotfiles config --local status.showUntrackedFiles no
```
You can also clone it without `--bare` for just a repo containing the files, if you don't want to automatically sync them.

## Usage
```
dotfiles add <file>
dotfiles commit -m "Changed <file>"
dotfiles push
```

`dotfiles` works like `git` for this repo, for example `dotfiles status`, `dotfiles pull`.
