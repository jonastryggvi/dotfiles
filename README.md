# My flavor of Mathias's dotfiles

## Installation

First, make sure that you have installed XCode from the app store, and install Virtual Box from https://www.virtualbox.org/wiki/Downloads

```bash
cd; curl -#L https://github.com/jonastyggvi/dotfiles/tarball/master | tar -xzv --strip-components 1 --exclude={README.md,bootstrap.sh,LICENSE-MIT.txt}
cd dotfiles
source bootstrap.sh
ruby -e "$(curl -fsSL https://raw.github.com/Homebrew/homebrew/go/install)"
# this might ask you to run as sudo, but don't! Try sudo brew doctor
brew bundle Brewfile
open init/digon.terminal
```
The last command will open a command line terminal, select preferences->Settings and find the digon profile, and make that default

Start Intellij IDEA, select configure and install these plugins; Node, Python, Ruby. Go to Preferences and enable the Dracula theme :)
```
