# Dotfiles of [tmaier][]

I use [homesick][] to manage my dotfiles.
You can check out [dotfiles.github.io][] for more information about this topic.

[tmaier]: http://tobiasmaier.info
[homesick]: https://github.com/technicalpickles/homesick
[dotfiles.github.io]: http://dotfiles.github.io/

## Dotfiles

### Install

```bash
gem install homesick
homesick clone tmaier/dotfiles
homesick symlink dotfiles
```

### Update

```bash
homesick pull dotfiles
```

## Sensible OS X defaults

When setting up a new Mac, you may want to set some sensible OS X defaults:

```bash
./.osx
```

## Install Homebrew formulae

1. Install [Homebrew](http://brew.sh)
1. Install [Brew Bundle](https://github.com/Homebrew/homebrew-bundle) with `brew tap Homebrew/bundle`
1. Run `cd ~ && brew bundle`

## Whats remaining?

1. Install [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)
2. Set up iTerm2
  ```
  rm ~/Library/Preferences/com.googlecode.iterm2.plist
  ln -s ~/.homesick/repos/dotfiles/preferences/com.googlecode.iterm2.plist ~/Library/Preferences/com.googlecode.iterm2.plist
  ```
