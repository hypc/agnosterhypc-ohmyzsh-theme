# AgnosterHypc for oh-my-zsh

AgnosterHypc is a [oh-my-zsh][] shell theme based on the [Powerline Vim plugin][] & [Agnoster Theme][].

It currently shows:

* Battery Life (in case of the laptop is not charging)
* Timestamp
* [nvm][] & [pyenv][] & [conda][]
* Current directory
* Git status
* User & Host status

## Installing

After installing [oh-my-zsh][]

```bash
git clone https://github.com/hypc/agnosterhypc-ohmyzsh-theme.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/themes/agnosterhypc

if [ "$(uname -s)" = "Darwin" ]; then
    sed -i '' 's|^ZSH_THEME=.*|ZSH_THEME=agnosterhypc/agnosterhypc|g' ~/.zshrc
else
    sed -i 's|^ZSH_THEME=.*|ZSH_THEME=agnosterhypc/agnosterhypc|g' ~/.zshrc
fi

# disable changeps1 if used conda
if command -v conda > /dev/null; then
    conda config --set changeps1 false
fi
```

[oh-my-zsh]: https://github.com/robbyrussell/oh-my-zsh
[Powerline Vim plugin]: https://github.com/Lokaltog/vim-powerline
[Agnoster Theme]: https://gist.github.com/agnoster/3712874
[nvm]: https://github.com/nvm-sh/nvm
[pyenv]: https://github.com/pyenv/pyenv
[pyenv-virtualenv]: https://github.com/pyenv/pyenv-virtualenv
[conda]: https://conda.io/
