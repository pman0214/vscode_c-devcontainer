# VSCode Remote Container C Development Environment

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> VSCode C development environment relying on Remote Container extension

## Table of Contents

- [Install](#install)
- [Usage](#usage)
- [Contribute](#contribute)
- [License](#license)

## Install

### Install Docker and VSCode

Install these mandatory tools.
- [Docker](https://www.docker.com) has been correctly installed and available in PATH.
- [VSCode](https://code.visualstudio.com) has been correctly installed.

### Install VSCode Extension

Install [Remote - Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) extension.

### Download and Extract

Download and extract the archive of this repository. Open the extracted directory with VSCode.
```bash
wget --no-check-certificate https://github.com/pman0214/vscode_c-devcontainer/archive/refs/heads/master.tar.gz -O - | tar zxv
```

Instead, you can download the archive of this repository using a Web browser and extract the archive with any unarchiver.

## Usage

```bash
code vscode_c-devcontainer
```
Instead of running the above command, you can open VSCode from the windows/mac menu and run "File > Open Workspace..." to specify the extracted `vscode_c-devcontainer` directory.

You will be asked to reopen the folder in a remote container. Answer `Reopen in Conainer`.
If you mistakenly answered `Don't Show Again...`, then press `F1` to open the Command Palette and execute `Remote-Containers: Reopen in Container`.
You can also run `Reopen in Container` from the bottom left green button.
For the first time of `Reopen in Container`, it might take long time to build and start the docker container.

Now you are in a docker container. Write your C code, build the code, and run the compiled file on the integrated terminal.
Note that you can make subdirectories to put C source code files.

Code runner is available, so you can use shortcut Ctrl+Alt+N (Ctrl+Option+N on mac) to run your code.

## Contribute

* Bugfix pull requests are welcome.

## License

All the source files are released under the MIT license. See `LICENSE.txt`.

* Copyright (c) 2021-2025 Shigemi ISHIDA
