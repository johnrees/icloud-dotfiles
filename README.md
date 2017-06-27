# icloud-dotfiles

Forked from https://github.com/searls/icloud-dotfiles

The basic gist of this:

1. Store dotfiles in iCloud Drive
2. Have a script that symlinks iCloud drive & dotfiles to my home directory and
    installs (or updates) the programs I use, such that it can be re-run gracefully

## Setup

### 1. Fetch the dotfiles and throw them in iCloud Drive

Fork this repo and clone it into your iCloud Drive as "dotfiles" like so:

```
$ git clone --recursive https://github.com/johnrees/icloud-dotfiles.git "~/Library/Mobile Documents/com~apple~CloudDocs/dotfiles"
```

### 2. Run the setup script

Now, run the initial setup script (which you can review
[here](https://github.com/johnrees/icloud-dotfiles/blob/master/bin/setup-new-mac)):

```
$ ~/Library/Mobile\ Documents/com~apple~CloudDocs/dotfiles/bin/setup-new-mac
```

In my case, this sets up my symlinks, installs/updates my brew formulas,
sets up Node & Ruby and then sources my bash profile.

