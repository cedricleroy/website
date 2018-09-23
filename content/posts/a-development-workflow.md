---
title: "A Development Workflow"
date: 2018-08-19T20:32:21-05:00
draft: false
---

From my first programming steps, I used a bunch of different IDEs to code, depending on the times and the
programming language used: `Borland C++`, `Code::Blocks` (for C), `Visual Studio` (C, C++), `Matlab IDE`,
`IDLE` (Python native IDE), `Eclipse` (With `PyDev` for `Python`), `Spyder`, `Sublime Text`, `Vim`, `VS Code`, etc.

This is somehow chronological. I lately used `VS Code` because of three main reasons: This is a great software from
Microsoft, I needed to work on Windows (unfortunately) and wanted something great for switching between languages.

Since I recentely came back to MacOS / Linux, I felt the need to restore my "old school" development workflow, with
`vim` and `tmux`. This is what this note is about.

## Terminals
* [iTerm2](https://iterm2.com/) on MacOS.
* [Terminator](https://gnometerminator.blogspot.com/) on Linux

## Vim
A couple of years now I have been using `Vim`. I still feel as a newbie considering the wide options it offers, but also feel
productive with it. I use it in the shell, but also with `Sublime Text` and `VS Code` thanks to the plugins.

`Vim` in the shell with some configuration and plugins is a killer tool for developping in Python.
![vim](/vim.png)

[Here](https://github.com/cedricleroy/config/blob/master/.vimrc) is my vim configuration file (`.vimrc`). Here is what is worth
mentionning:

* I use [vundle](https://github.com/cedricleroy/config/blob/master/.vimrc) as vim package manager.
  Installing a plugin is simple: ``:PluginInstall``
* My leader key is `\`
* Plugins:
  * Nerdtree (left of the screenshot above)
  * Vim colorschemes (I usually use `molokai`).
  * `ctrp`: Fuzzy file finder. I tend to use `fzf` more now.
  * Vim airline with themes for status/tabline. 
  * `ale` for async linting.
  * `jedi` for Python autocompletion.
  * `ack` as search tool.
  * `fzf` as main fuzzy file finder.
* A few key binding:
  * `jj` as second `ESC`.
  * `TAB` with `.` (repeat)
  * `CTRL+N` to toggle nerdtree
  * leader + f to trigger `fzf` for fuzzy finding (`:Files`).
  * leader + q to trigger `fzf` with git filtering (`:GFiles`).
