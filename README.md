# System Configuration Management

This repository provides a collection of scripts and configuration files for managing system settings and applications.
Note: This repository is a work in progress and is intended for personal use.

## Requirements

GNU Stow: https://www.gnu.org/software/stow/
dconf: a system for storing and retrieving configuration data

## Usage Dotfiles

- Install GNU Stow on your system.
- Clone this repository to ~/dotfiles directory.
- Run stow in directory to manage system configuration files.

## Usage Dumpfiles

Use dconf to manage application settings:

backup gnome shell extension settings

```bash
cd ~/dotfiles
dconf dump /org/gnome/shell/extensions/ > gnome_shell_extensions.dump
```

restore gnome shell extension settings

```bash
cd ~/dotfiles
dconf load /org/gnome/shell/extensions/ < gnome_shell_extensions.dump
```
