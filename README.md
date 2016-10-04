# Simple plugin manager

This is my personal Vim plugin manager. It comes in the form of a Bash shell
script, and no Windows support is planned.

## Requirements

* Bash
* Git

## How to install

The first thing to do is to backup your `.vim` folder, just in case, then when
you've put `virgo` in your PATH, install your first vim plugin with:

```
$ virgo install ctrlpvim/ctrlp.vim
```

You must call the `load` function within your `.vimrc` and then activate the
filetype and indent plugin. You can use these lines as template:

```
call virgo#load()
filetype indent plugin on
syntax on
```

## How to install a plugin

Supported Vim plugins comes as a Git repository. If the plugin you are
installing comes from Github, you can simply use the abbreviated syntax like
this:

```
$ virgo install kien/ctrlp.vim
```

If the plugin comes from a different source, you can just use the URL:

```
$ virgo install http://my.server.here.it/vimawesome
```

## How to update the plugins

```
$ virgo update
```

## How to list the installed plugins

```
$ virgo list
```

## How to remove an installed plugin

```
$ virgo remove ctrlp.vim
```
