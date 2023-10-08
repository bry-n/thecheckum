---
title: Neovim Cheat Sheet
slug: /neovim-cheat-sheet/
tags: ['Cheatsheet']
date: 2022-10-02T11:31:46-04:00
draft: false
# layout: 
# description: 
# tags: 
# icon: 
# thumbnail: 
    # url: 
    # author: 
    # authorURL: 
    # origin: 
    # originURL: 
---

## What Is Neovim
Neovim is a highly customizable VIM-based text editor. Runs on Linux, macOS, & Windows

## Neovim Site
Instructions for installing Neovim can be found at [https://Neovim.io](https://neovim.io/)

## How to Use
Using a terminal type `nvim` followed by the file name. A new file will be created if it doesn't already exist.  
`nvim example.txt`  

## Helpful Key Commands

{{< table "table-striped" >}}
| **Key Command**  | **Description**              |
| ------------ |:---------------------------------|
| esc          | Escape Mode                      |
| i            | Insert Mode                      |
|:             | Commandline Mode                 |
| h            | Move Cursor Left                 |
| j            | Move Cursor Up                   |
| k            | Move cursor Down                 |
| l            | Move Cursor Left                 |
| :w           | Save                             |
| :q           | Quit                             |
| esc+u        | Undo                             |
| dw           | Delete Word                      |
| dd           | Delete Entire Line               |
| p            | Paste Last Deleted Word or Line  |
| r+key        | Replace Any Character            |
{{< /table >}}