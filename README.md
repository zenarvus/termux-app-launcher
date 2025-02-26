# Termux App Launcher
An application launhcer for Termux, without hacking the apk file.

Tested on android 11.

## Dependencies
- [fzf](https://github.com/junegunn/fzf): Required. Used for listing all installed applications.
- [AnyHome](https://github.com/tytydraco/AnyHome)/[TermuxLauncher](https://github.com/amsitlab/termuxlauncher): Optional, but recommended. Used for making Termux the default home launcher.
- `am`, `cmd` and `aapt` commands in Termux.

## Installation
```sh
wget https://raw.githubusercontent.com/zenarvus/termux-app-launcher/refs/heads/main/app-launcher -O ~/.local/bin/app-launcher && chmod +x ~/.local/bin/app-launcher
```

Do not forget that `~/.local/bin/` should be in the `PATH`. Put this code in your `.bashrc` file:
```sh
export PATH=$PATH:~/.local/bin
```

## Usage
```
help: lists all available commands.

select: spawn fzf to select and launch an application.

generate: generate a list of currently installed applications.
```
