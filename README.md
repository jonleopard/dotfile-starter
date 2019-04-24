# Welcome to the dotfile starter!

Let's start off with symlinking some dotfiles with GNU Stow! First, make clone this repo into your home directory:

```
git clone https://github.com/jonleopard/dotfiles_starter.git && cd dotfiles_starter
```

If you don't have the following set up, go ahead and do so:

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

There is just one directory in this repo `zsh`. We will add more later. `zsh` contains a zsh dotfile named `.zshrc_test`. Once you run stow on the zsh directory, you should see that dotfile show up in your home directory. Try it out:

Run `stow zsh`, and then look at your home directory again

You can also avoid using stow altogether if you wish. But as your environment grows, its best to use some sort of dotfile manager or symlink farm manager to help you keep everything clean and organized. I chose stow because its very tiny (no dependencies, I believe?), and simple to use once you wrap your head how it works.

I wrote a small [blog post](https://jonleopard.com/blog/dotfile-management-with-gnu-stow) on stow a while back, feel free to check it out.


[logo]: .github/dotfile-starter.png

