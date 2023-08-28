---
title: Getting Started
author: doctorfree
date: 2023-07-20 16:20:00 +0800
tags: [data, benchmarks, stats, info, initialization]
pin: true
img_path: "/posts/20230720"
---

## LazyIde Neovim Configuration

See the [LazyIde Install section](https://ide.lazyman.dev/install) to install
the `LazyIde` Neovim configuration.

## Nvims Configuration Selection

Once the `lazyman` command and `LazyIde` configuration are installed,
use the `nvims` command to select and open the `LazyIde` Neovim configuration.
This will automatically alias `vi` to use Neovim with the `LazyIde` config.

## Persistent nvim alias

Optionally, create a shell alias for `vi` or `nvim` to use the `LazyIde` Neovim
configuration. To do so, add something like the following to your shell
initialization file (typically `~/.bashrc` for Bash users or
`~/.zshrc` for Zsh users).

```bash
alias nvim="NVIM_APPNAME=lazyman/LazyIde nvim"
```

## NVIM_APPNAME environment variable

In Neovim 0.9+ the environment variable `NVIM_APPNAME` is used to determine
which Neovim configuration is used. Use this environment variable to
automatically tell Neovim to use `LazyIde`. To do so, add the following
to your shell initialization file:

```bash
export NVIM_APPNAME="lazyman/LazyIde"
```
