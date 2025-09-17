# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a dotfiles repository for macOS/Linux development environment configuration, primarily focused on Le Wagon bootcamp setup. It contains configuration files for shell (zsh), git, Ruby, and Sublime Text.

## Key Commands

### Initial Setup
```bash
# Install all dotfiles and create symlinks
./install.sh

# Configure git identity
./git_setup.sh
```

### Git Operations
- Main branch: `master`
- Remote upstream: `git@github.com:lewagon/dotfiles.git`

## Architecture & Structure

- **Shell scripts**:
  - `install.sh`: Creates symlinks from dotfiles to home directory, installs zsh plugins, configures Sublime Text
  - `git_setup.sh`: Sets up git user identity and validates GitHub email configuration

- **Configuration files**:
  - `zshrc`: Oh-My-Zsh configuration with rbenv, nvm, pyenv paths and custom plugins
  - `aliases`: Custom command aliases for IP info and HTTP server
  - `gitconfig`, `gitignore`: Git configuration
  - Ruby configs: `gemrc`, `irbrc`, `rspec`
  - Editor configs: Sublime Text preferences and Package Control settings

## Development Environment

- **Shell**: Zsh with Oh-My-Zsh (robbyrussell theme)
- **Ruby**: rbenv for version management
- **Node**: nvm for version management
- **Python**: pyenv for version management
- **Editor**: Sublime Text as default editor for git and bundler
- **Database**: PostgreSQL 16 configured in PATH