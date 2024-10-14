# To-do List Upon Getting a New MacBook

## Personal Preferences
* Trackpad
  * Look up & data detectors: Tap with three fingers
  * Tap to click: tick
  * Tracking speed: Fast
* Accessibility - Point control - Trackpad Options - Eable dragging: three finger drag 
  * for three finger drag
* Keyboard - Keyboard navigation: tick
  * *Use keyboard navigation to move focus between controls. Press the Tab key to move focus forward and Shift Tab to move focus backward.*
  * this is to use **tab** to choose between dialogue box buttons

## Dev Essentials
### Install Command Line Developer Tools & Git
```
~ % xcode-select --install # to trigger the prompt to install. It takes a few minutes.
~ % xcode-select -p # to verify installation success
/Library/Developer/CommandLineTools
~ % git --version
git version 2.39.3 (Apple Git-146)
```
See [reference](https://www.freecodecamp.org/news/install-xcode-command-line-tools/).

### Homebrew
1. `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
    * if failed, check the most up to date command on its official doc: https://brew.sh/
    * This will automatically install zsh and use it as default shell
2.  Add Homebrew to your PATH:
    ```
    echo >> ~/.zprofile
    echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zprofile
    eval "$(/opt/homebrew/bin/brew shellenv)"
    ```
3. `brew -v`


### iTerm2 and oh-my-zsh
This guys's reference: https://catalins.tech/improve-mac-terminal.

oh-my-zsh github repo and README: https://github.com/ohmyzsh/ohmyzsh

1. install zsh `brew install zsh` , `zsh --version`
2. change default shell to zsh if needed `chsh -s /bin/zsh`
3. install iterm2 `brew install --cask iterm2`
4. iTerm2 > Settings > Profiles > Colors > Color Presets -> Tango Light
5. install oh-my-zsh `sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`
6. change zsh home directory before proceeding on installing plugins `export ZSH="$HOME/.oh-my-zsh"`

#### [oh-my-zsh handy plugins](https://gist.github.com/dogrocker/1efb8fd9427779c827058f873b94df95)
1. Run command anywhere to download the plugins into ZSH's own directory
   ```
   # auto suggestion
   git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH/custom/plugins/zsh-autosuggestions
 
   # syntax highlight
   git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH/custom/plugins/zsh-syntax-highlighting
   ``` 
2. `vi ~/.zshrc` to check the current zsh config file and add the plugins
   ```
   plugins=(
     git
     zsh-autosuggestions 
     zsh-syntax-highlighting
     web-search
   )
   ```
3. Exit and reopen iTerm2

   
### Intellij
Download Ultimate: https://www.jetbrains.com/idea/download/#section=mac

