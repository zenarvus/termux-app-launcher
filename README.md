# Termux App Launcher
A simple android application launcher script for Termux.

Tested on android 11.

## Requirements
- [fzf](https://github.com/junegunn/fzf): To list the applications.
- `aapt`: To extract the application label.
- `am`: To launch the application.
- `cmd`: To list the installed packages and paths.

The last two are probably already installed.

For the first two, use this command:
```sh
pkg install fzf aapt -y
```

## Installation
```sh
mkdir -p ~/.local/bin && wget https://raw.githubusercontent.com/zenarvus/termux-app-launcher/refs/heads/main/app-launcher -O ~/.local/bin/app-launcher && chmod +x ~/.local/bin/app-launcher
```

Do not forget that `~/.local/bin/` should be in the `PATH`. Put this code in your `.bashrc` file:
```sh
export PATH=$PATH:~/.local/bin
```

## Usage
```
help: lists all available commands.

select: spawns fzf to select and launch an application.

generate: generates a list of currently installed applications.
```

## Recommendations
You can also make Termux your default home screen with one of these cool applications:
- [AnyHome](https://github.com/tytydraco/AnyHome) by [@tytydraco](https://github.com/tytydraco) (Works on newer versions of android)
- [TermuxLauncher](https://github.com/amsitlab/termuxlauncher) by [@amsitlab](https://github.com/amsitlab) 
- [Termux:Home](https://github.com/zenarvus/termux-home) by [@zenarvus](https://github.com/zenarvus)
