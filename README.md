# AgnosterHypc for oh-my-zsh

AgnosterHypc is a [oh-my-zsh][] shell theme based on the [Powerline Vim plugin][] & [Agnoster Theme][].

It currently shows:

* Battery Life (in case of the laptop is not charging)
* Timestamp
* [nvm][] & [pyenv][] & [conda][]
* Current directory
* Git status
* User & Host status

## Pre Install

```bash
# disable changeps1 when used conda
conda config --set changeps1 false
```

## Installing

After installing [oh-my-zsh][]

```bash
# Put the file `agnosterhypc.zsh-theme` in `$ZSH_CUSTOM/themes/`:
wget -O $ZSH_CUSTOM/themes/agnosterhypc.zsh-theme https://raw.githubusercontent.com/hypc/agnosterhypc-ohmyzsh-theme/master/agnosterhypc.zsh-theme
# Configure the theme in your `~/.zshrc` file:
sed -i 's/^ZSH_THEME=.*/ZSH_THEME="agnosterhypc"/g' ~/.zshrc
```

[oh-my-zsh]: https://github.com/robbyrussell/oh-my-zsh
[Powerline Vim plugin]: https://github.com/Lokaltog/vim-powerline
[Agnoster Theme]: https://gist.github.com/agnoster/3712874
[nvm]: https://github.com/nvm-sh/nvm
[pyenv]: https://github.com/pyenv/pyenv
[pyenv-virtualenv]: https://github.com/pyenv/pyenv-virtualenv
[conda]: https://conda.io/
