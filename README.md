# st - simple terminal

st is a simple terminal emulator for X which sucks less.

This repository is just a fork of [st][https://st.suckless.org/] with some patches applied on top.

## Included Patches

## Requirements

In order to build st you need the Xlib header files.

## Installation

Edit `config.mk` to match your local setup (st is installed into
the `/usr/local` namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

```sh
make clean install
```

## Running st

If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

```sh
tic -sx st.info
```

See the man page for additional details.

## Updating from upstream suckless st

In order to pull the latest changes from upstream st:

1. Set upstream repository: `git remote add upstream https://git.suckless.org/st`
1. Pull latest changes: `git pull upstream master`

## Credits

Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

