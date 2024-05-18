 # Dotfiles

This directory contains the dotfiles for my system

Setup stolen from Dreams of Autonomy, great content!
https://www.youtube.com/watch?v=y6XCebnB9gs

## Requirements

Ensure you have the following installed on your system

### Git
( should already be installed on ubuntu )

```
sudo apt install git
```

### Stow

```
sudo apt-get install stow
```

## Installation

First, check out this repo and navigate to the dotFile folder

```
$ git git@github.com:DeCatNiels/ubuntu_setup.git
$ cd ubuntu_setup/dotFiles
```

then use GNU stow to create symlinks

```
$ stow -t ~ .
```