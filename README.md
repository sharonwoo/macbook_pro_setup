# macbook_pro_setup
Because this is the third logic board failure in a year.
* Jun 2019: display replacement (orange splotches) 
* Jan 2020: display and top case replacement
* May 2020: logic board replacement (relating to TouchID and SMC reset)
* Jul 2020: ?????? hardware failure after pressing the power button

25 Jul 2020: set up new 16" after replacement; collection of 15" on 28 Jul

## Install Brew

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

## Brew cask installs
```
brew cask install firefox ungoogled-chromium telegram iterm2 blisk vlc transmission little-snitch visual-studio-code atom ... 
```
* [A good, somewhat outdated list for manual installs](https://sourabhbajaj.com/mac-setup/Homebrew/Cask.html). Configure AWS-cli/Heroku etc as needed.
* TODO: port over as a bash script (see [this](https://gist.github.com/brunofbrito/13c29c9b1f7a833066a98522d4b826f7)). Right now things are minimal enough that you don't really need it. 

## Configure Chromium with adblocker specials
* Install [Chromium Web Store](https://ungoogled-software.github.io/ungoogled-chromium-wiki/faq#can-i-install-extensions-or-themes-from-the-chrome-webstore) and follow these instructions
* Install plugins: Decentraleyes | UB Origin | UMatrix | [Next Step for Trello](https://chrome.google.com/webstore/detail/next-step-for-trello/iajhmklhilkjgabejjemfbhmclgnmamf?hl=en)

## Configure iterm2 and omz
* ```brew install zsh```
* Install oh-my-zsh ```sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"``` and optionally the Darcula theme. [Special thanks](https://medium.com/ayuth/iterm2-zsh-oh-my-zsh-the-most-power-full-of-terminal-on-macos-bdb2823fb04c). You might need to fix this issue ```[oh-my-zsh] Insecure completion-dependent directories detected:``` by editing zshrc.
* Install [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting). Enter ```open ~/.oh-my-zsh``` and git clone the repo. Then edit zshrc with ```nano ~/.zshrc```, making sure zsh-syntax-highlighting is the last plugin in plugins, and ```source ~/.zshrc``` to complete changes.

## Configure BTT
[GoldenChaos](https://community.folivora.ai/t/goldenchaos-btt-the-complete-touch-bar-ui-replacement/1281)

## Other programs
* Devonthink
* Little Snitch 
* Fantastical
* Omnifocus 
* Notability
* Atom plugins: platformio-ide-terminal and python-autocomplete

## Conda, because it's a lot of trouble to migrate everything to something else 

[Thank god I'm still on Mojave](https://stackoverflow.com/questions/58291108/conda-not-found-after-upgrading-to-macos-catalina).
Installing Miniconda from .pkg and then creating a full environment seems to work fine now with zsh as shell. Use ```echo $SHELL``` to check it's indeed zsh that's in play. And [why I'm sticking to Conda for now](https://stackoverflow.com/questions/54834579/specific-reasons-to-favor-pip-vs-conda-when-installing-python-packages).
