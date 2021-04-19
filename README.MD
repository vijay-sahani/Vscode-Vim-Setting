# Vscode vim settings

<h2 align="center"><img src="https://raw.githubusercontent.com/VSCodeVim/Vim/master/images/icon.png" height="128"><br>VSCodeVim</h2>
<p align="center"><strong>Vim emulation for Visual Studio Code</strong></p>

[![](https://vsmarketplacebadge.apphb.com/version/vscodevim.vim.svg)](http://aka.ms/vscodevim)
[![](https://vsmarketplacebadge.apphb.com/installs-short/vscodevim.vim.svg)](https://marketplace.visualstudio.com/items?itemName=vscodevim.vim)
[![](https://github.com/VSCodeVim/Vim/workflows/build/badge.svg?branch=master)](https://github.com/VSCodeVim/Vim/actions?query=workflow%3Abuild+branch%3Amaster)
[![](https://img.shields.io/badge/vscodevim-slack-blue.svg?logo=slack)](https://vscodevim.herokuapp.com/)

VSCodeVim is a Vim emulator for [Visual Studio Code](https://code.visualstudio.com/).

## ⚙️ Settings

## Basic

```json
 "vim.easymotion": true,
  "vim.incsearch": true,
  "vim.useSystemClipboard": true,
  "vim.useCtrlKeys": true,
  "vim.hlsearch": true,
  "vim.overrideCopy": true,
  "vim.leader": "<space>",
  "vim.handleKeys": {
    "<C-a>": false,
    "<C-f>": false,
    "<C-c>": false,
    "<C-v>": false,
    "<C-x>": false,
    "<C-y>": false
  },
```

## Insert Mode

```json
{
  "vim.insertModeKeyBindings": [
    {
      "before": ["j", "j"],
      "after": ["<Esc>"]
    },
    {
      "before": ["j", "k"],
      "after": ["<Esc>"]
    },
    {
      "before": ["k", "j"],
      "after": ["<Esc>"]
    }
  ]
}
```

## Normal Mode

```json
"vim.normalModeKeyBindingsNonRecursive": [
    {
      "before": ["<leader>", "d"],
      "after": ["d", "d"]
    },
    // Copy a line
    {
      "before": ["c"],
      "after": ["y", "y"]
    },
    //Delete a character before
    {
      "before": ["d"],
      "after": ["X"]
    },
    {
      "before": ["<C-n>"],
      "commands": [":nohl"]
    }
  ],
```

## Visual Mode

```json
 "vim.visualModeKeyBindings": [
    // In visual mode i goes to insert mode
    {
      "before": ["i"],
      "after": ["<Esc>", "i"]
    },
    {
      "before": ["c"],
      "after": ["y", "y"]
    }
  ],
```

<p align="center"><strong>Feel free to edit/make any changes ❤</strong></p>
