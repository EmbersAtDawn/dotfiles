# Dotfiles

Currently includes:
- .zshrc
- .gitconfig


# macOS Requirements
Install [Homebrew](https://brew.sh/)
```shell
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Install dependencies:
```shell
$ brew install zsh-syntax-highlighting
$ brew install zsh-autosuggestions
$ brew coreutils
```

Change `ls` aliased commands to use `gls`:
```zsh
alias ls='gls --color=auto --human-readable --group-directories-first --classify'
alias ll='gls --color=auto --human-readable --group-directories-first --classify -l'
alias lla='gls --color=auto --human-readable --group-directories-first --classify -la'
```

Change sources for zsh extensions at the end of `.zshrc` file:
```zsh
source /opt/homebrew/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh
source /opt/homebrew/share/zsh-autosuggestions/zsh-autosuggestions.zsh
```

Reload the `.zshrc` configuration:
```shell
$ source .zshrc
```
