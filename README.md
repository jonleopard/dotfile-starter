# Welcome to the dotfiles example repo!

Let's start off with symlinking some dotfiles with GNU Stow! If you don't have thefollowing set up, go ahead and do so:

## [homebrew](https://brew.sh/)
A package manager for Mac

```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

## [zsh](http://zsh.sourceforge.net/)
A bash shell alternative that includes things like file globbing, git command completion, among others.
```
brew install zsh && sudo dscl . -create /Users/$USER UserShell /usr/local/bin/zsh

``` 

## [stow](https://www.gnu.org/software/stow/)
A symlink farm manager. This helps us keep our home `/` directory clean. Alternatives exists and I encourage you to compare them to find what you like.
```
brew install stow

```



## Practice

Now that all that is installed, we can start symlinking some dotfiles. To demonstrate this example, load up a finder and navigiate to your home directory. Make sure invisable files are displaying with either ` CMD + SHIFT + .` or run this `defaults write com.apple.finder AppleShowAllFiles YES`.

There are three directories in this repo.

Run `stow zsh`, and then look at your home directory again. You should now see it 





