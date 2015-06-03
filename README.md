# My flavor of Mathias's dotfiles

## Installation

First, make sure that you have installed XCode from the app store, and install Virtual Box from https://www.virtualbox.org/wiki/Downloads

```bash
cd; curl -#L https://github.com/jonastyggvi/dotfiles/tarball/master | tar -xzv --strip-components 1 --exclude={README.md,bootstrap.sh,LICENSE-MIT.txt}
cd dotfiles
source bootstrap.sh

ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew install rbenv ruby-build
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bash_profile
rbenv install 2.1.6

open init/digon.terminal
```
The last command will open a command line terminal, select preferences->Settings and find the digon profile, and make that default
