New Mac To-do List

## Homebrew
1. Xcode command line tool if not already exist `xcode-select --install`
2. `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
3. `brew -v`

## iTerm2 and oh-my-zsh
This guys's reference: https://catalins.tech/improve-mac-terminal.

oh-my-zsh github repo and README: https://github.com/ohmyzsh/ohmyzsh

1. `brew install zsh | chsh -s /bin/zsh`
2. `brew install --cask iterm2`
3. `sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`
4. iTerm2 > Preferences > Profiles > Colors > Color Presets -> Tango Light

### oh-my-zsh handy plugins
https://gist.github.com/dogrocker/1efb8fd9427779c827058f873b94df95
* auto suggestion: `git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions`
* syntax highlight: `git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting`

vi ~/.zshrc
```
plugins=(
  git
  zsh-autosuggestions 
  zsh-syntax-highlighting
  web-search
)
```

## Intellij
jetbrains.com/idea/download/#section=mac
