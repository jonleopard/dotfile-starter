# Welcome to the dotfiles example repo!

Let's start off with symlinking some dotfiles with GNU Stow! If you don't have thefollowing set up, go ahead and do so:

##[homebrew](https://brew.sh/)
A package manager for Mac

```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

##[zsh](http://zsh.sourceforge.net/)
A bash shell alternative that includes things like file globbing, git command completion, among others.
```
brew install zsh && sudo dscl . -create /Users/$USER UserShell /usr/local/bin/zsh

``` 

##[stow](https://www.gnu.org/software/stow/)
A symlink farm manager. This helps us keep our home `/` directory clean. Alternatives exists and I encourage you to compare them to find what you like.
```
brew install stow

```





