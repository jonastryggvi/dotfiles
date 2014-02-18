# My flavor of Mathias's dotfiles

## Installation

First, make sure that you have installed XCode from the app store, and install Virtual Box from https://www.virtualbox.org/wiki/Downloads

```bash
cd; curl -#L https://github.com/jonastyggvi/dotfiles/tarball/master | tar -xzv --strip-components 1 --exclude={README.md,bootstrap.sh,LICENSE-MIT.txt}
cd dotfiles
source bootstrap.sh
./.osx
ruby -e "$(curl -fsSL https://raw.github.com/Homebrew/homebrew/go/install)"
# this might ask you to run as sudo, but don't! Try sudo brew doctor
brew bundle Brewfile
open init/digon.terminal
```
The last command will open a command line terminal, select preferences->Settings and find the digon profile, and make that default

Go get Java 7 if you want.. no need, intellij has a bundled JRE.
http://www.oracle.com/technetwork/java/javase/downloads/jdk7-downloads-1880260.html

Start Intellij IDEA, select configure and install these plugins; Node, Python, Ruby. Go to Preferences and enable the Dracula theme :)

Install Ruby via RVM (Ruby Version Manager)
```bash
curl -sSL https://get.rvm.io | bash -s stable --ruby
# or if you had rvm installed but no proper ruby, then 
# rvm install ruby
# rvm use ruby --default

gem install berkshelf
brew tap phinze/homebrew-cask
brew install brew-cask
brew install cask vagrant

vagrant install vagrant-berkshelf
vagrant install vagrant-omnibus

brew install node
npm install -g nodemon
npm install -g express
```
