### Bashmarks is a shell script that allows you to save and jump to commonly used directories. Now supports tab completion.

Credits: this is a fork from the original repo: [huyng/bashmarks](https://github.com/huyng/bashmarks), the main change is changing the s,g,p,d,l command to st,gt,pt,dt,lt.

## Install

1. git clone https://github.com/bofeng/bashmarks.git
2. cd bashmarks
3. make install
4. source **~/.local/bin/bashmarks.sh** from within your **~.bash_profile** or **~/.bashrc** or **~/.zshrc** (if using zsh) file

## Shell Commands

    st <bookmark_name> - Saves the current directory as "bookmark_name"
    gt <bookmark_name> - Goes (cd) to the directory associated with "bookmark_name"
    pt <bookmark_name> - Prints the directory associated with "bookmark_name"
    dt <bookmark_name> - Deletes the bookmark
    lt                 - Lists all available bookmarks

## Example Usage

    $ cd /var/www/
    $ st webfolder
    $ cd /usr/local/lib/
    $ st locallib
    $ lt
    $ gt web<tab>
    $ gt webfolder

## Where Bashmarks are stored

All of your directory bookmarks are saved in a file called ".sdirs" in your HOME directory.
