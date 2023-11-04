---
title: Tmux Cheat Sheet
slug: /tmux-cheat-sheet/
tags: ['Cheatsheet']
date: 2023-11-04
draft: false
# layout: 
# description: 
tags: cheatsheet 
# icon: 
thumbnail: img/cheatsheet.png
    # url: 
    # author: 
    # authorURL: 
    # origin: 
    # originURL: 
---

## What Is Tmux
It's a command line tool which will allow you to run multiple programs.

## Tmux Site
Instructions for installing Tmux can be found at [https://github.com/tmux/tmux/wiki](https://github.com/tmux/tmux/wiki)

## How to Use
Using a terminal type `tmux` and you'll be dropped into a Tmux session.  

## Helpful Key Commands

{{< table "table-striped" >}}
| **Key Command**  | **Description**   |
|---|---|
| tmux | Start a session |
| tmux new -s Test | Start a new session called Test   |
| tmux ls | List any active sessions |
| tmux attach -t # | Connect to an active session (# = session number) |
| tmux rename-session -t # new_name | Rename a session (# = session number)  |
| exit or ctrl-d | Exit an active session, window, or pane |
| ctrl-b then shift-5 | Create another pane |
| ctrl-b then arrow keys | Move between panes |
| ctrl-b then c | Create a new window |
| ctrl-b then n | Move to the next window |
| ctrl-b then p | Move to the previous window |
| ctrl-b then d | Detach current session |
| ctrl-b then D | Detach session of choice |
{{< /table >}}