# Termux App Launcher
A simple android application launcher script for Termux.

Tested on android 11.

## Requirements
- [fzf](https://github.com/junegunn/fzf): To list the applications.
- `am`: To launch the application.
- `cmd`: To list the installed packages and paths.
- `aapt`: To extract the application label.

The last three are probably already installed.

For the first one, use this command:
```sh
pkg install fzf -y
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
- [Termux:Home](https://github.com/zenarvus/termux-home) by [@zenarvus](https://github.com/zenarvus)
- [AnyHome](https://github.com/tytydraco/AnyHome) by [@tytydraco](https://github.com/tytydraco)
- [TermuxLauncher](https://github.com/amsitlab/termuxlauncher) by [@amsitlab](https://github.com/amsitlab)
