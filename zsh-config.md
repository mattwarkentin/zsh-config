# Terminal and zsh Setup

## Preamble

This README describes how I have setup my terminal and zsh. This document assumes you use Homebrew as your Mac OS package manager. If you do not already have [Homebrew](https://brew.sh/) installed run the following command:

> `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

## Step-by-Step Guide:

- Install [iTerm2](https://iterm2.com/)

  - `brew install --cask iterm2`

  - Main Custom Preferences
    - Appearance
      - Theme: Dark (High Contrast)
      - Tab bar location: Top
      - Status bar location: Bottom
    - Profiles > Text
      - Underline
      - Font: FiraCode Nerd Font Mono
      - Font: Use ligatures
    - Profiles > Window
      - Transparency: 5
      - Blue: 10
    - Profiles > Session > Configure Status Bar
      - Status bar enabled
      - Choose whatever you want for status bar things...

- Install `oh-my-zsh`

  - `sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

- zsh plugins
  - [zsh-completions](https://github.com/zsh-users/zsh-completions)
    - ` git clone https://github.com/zsh-users/zsh-completions ${ZSH_CUSTOM:-${ZSH:-~/.oh-my-zsh}/custom}/plugins/zsh-completions`

  - [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)
    - `git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting`

  - [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions)
    - `git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions`

- Install [Exa](https://github.com/ogham/exa) - a modern replacement for ls

  - `brew install exa`

- Install Nerd fonts

  - Download `https://github.com/ryanoasis/nerd-fonts/releases/download/v2.1.0/FiraCode.zip`

  - Unzip file and install font on your machine via:
    - Open Mac Font Book app and drag and drop `Fira Code Retina Nerd Font Complete Mono.otf`

- Install [bat](https://github.com/sharkdp/bat) - A cat(1) clone with syntax highlighting and Git integration.

  - `brew install bat`

- Install an iTerm Theme

  - https://github.com/mbadolato/iTerm2-Color-Schemes

  - I use the Peppermint theme which can be downloaded by going into the `schemes/` folder and saving the `Peppermint.itermcolors` file to disk and then importing this theme into iTerm2 via:
    - Profiles > Colors > Color Presets... > Import

- Configure your `.zshrc` and setup aliases
