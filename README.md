stac-dot-files
==============

All my dot files. They are commons for GNU/Linux and MacOSX.

Installation
------------

### Automatic

I need to create a small script for this repetitive operation.

### Manual

#### Getting the config files and plugins

First clone this repo in your home. I usually clone it in ~/.stac-dot-files.

    git clone https://github.com/stac47/stac-dot-files.git .stac-dot-files

Then, go to this folder and download all the git submodules:

    cd .stac-dot-files
    git submodule update --recursive --init

#### Creating symbolic links to the config files

Finally, simply symlink all the files you need:

    ln -s ~/.stac-dot-files/.bashrc ~/.bashrc
    ln -s ~/.stac-dot-files/.bash_profile ~/.bash_profile
    ln -s ~/.stac-dot-files/.bash_logout ~/.bash_logout
    ln -s ~/.stac-dot-files/.gitconfig ~/.gitconfig
    ln -s ~/.stac-dot-files/.gitignore_global ~/.gitignore_global
    ln -s ~/.stac-dot-files/.irbrc ~/.irbrc
    ln -s ~/.stac-dot-files/.vimrc ~/.vimrc
    ln -s ~/.stac-dot-files/.vim ~/.vim
    ln -s ~/.stac-dot-files/scripts/battery/bin/battery ~/battery

Regarding tmux, as it is a bit more difficult to copy to the Mac OSX clipboard,
we have two choices of ".tmux.conf" file:

    ln -s ~/.stac-dot-files/.tmux.conf.osx ~/.tmux.conf
    or
    ln -s ~/.stac-dot-files/.tmux.conf.linux ~/.tmux.conf
