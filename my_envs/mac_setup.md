# Macbook Dev Setup

## Tools

### Dev tools
- Xcode
- xcode-select --install
- brew

### Terminal & Shells & IDE
- iTerm2
- zsh
    - oh-my-zsh
    - theme
    - zsh-autosuggestions
    - zsh-syntax-highlighting
- bash
    - oh-my-bash
- fish
    - oh-my-fish
- vscode
    - setting.json
    ```json
        {
            "terminal.external.osxExec": "iTerm.app",
            // "terminal.integrated.fontFamily": "ProFont for Powerline",
            // "terminal.integrated.fontFamily": "Space Mono for Powerline",
            // "terminal.integrated.fontFamily": "'Source Code Pro for Powerline', 'Hack Nerd Font'", 
            "terminal.integrated.fontFamily": "Meslo LG M DZ for Powerline",
            "workbench.colorTheme": "Visual Studio Dark"
        }
    ```
    - extensions: vim & markdown & ...
- vim
    - config:  ~/.vimrc
    ```vim
        " Disable compatibility with vi which can cause unexpected issues.
        set nocompatible

        " Enable type file detection. Vim will be able to try to detect the type of file in use.
        filetype on

        " Enable plugins and load plugin for the detected file type.
        filetype plugin on

        " Load an indent file for the detected file type.
        filetype indent on

        " Turn syntax highlighting on.
        syntax on
    ```