# macbook_pro_setup
Because this is the third logic board failure in a year.

## Install Brew

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

## Brew cask installs
```
brew cask install firefox ungoogled-chromium telegram iterm2 blisk vlc transmission little-snitch visual-studio-code atom ... 
```
* [A good, somewhat outdated list for manual installs](https://sourabhbajaj.com/mac-setup/Homebrew/Cask.html). Configure AWS-cli/Heroku etc as needed.
* TODO: port over as a bash script (see [this](https://gist.github.com/brunofbrito/13c29c9b1f7a833066a98522d4b826f7)).

## Configure Chromium with adblocker specials
* Install [Chromium Web Store](https://ungoogled-software.github.io/ungoogled-chromium-wiki/faq#can-i-install-extensions-or-themes-from-the-chrome-webstore) and follow these instructions
* Install plugins: Decentraleyes | UB Origin | UMatrix | [Next Step for Trello](https://chrome.google.com/webstore/detail/next-step-for-trello/iajhmklhilkjgabejjemfbhmclgnmamf?hl=en)

## Configure iterm2 and omz
* ```brew install zsh```
* Install oh-my-zsh ```sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"``` and optionally the Darcula theme. [Special thanks](https://medium.com/ayuth/iterm2-zsh-oh-my-zsh-the-most-power-full-of-terminal-on-macos-bdb2823fb04c). You might need to fix this issue ```[oh-my-zsh] Insecure completion-dependent directories detected:``` by editing zshrc.
* Install [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting). Enter ```open ~/.oh-my-zsh``` and git clone the repo. Then edit zshrc with ```nano ~/.zshrc```, making sure zsh-syntax-highlighting is the last plugin in plugins, and ```source ~/.zshrc``` to complete changes.

## Other programs
* Devonthink
* Little Snitch 
* Fantastical
* Omnifocus 
* Notability
