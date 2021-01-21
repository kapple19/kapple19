---
title: Coding on Chrome OS
author: Aaron Kaw
---

# Purpose
This markdown file is created to record how I manage with coding on the Chrome OS system.

## Context
| Feature | Detail |
|---|---|
| CPU | arm64 |

# Linux
* Chrome OS has beta support for linux. The [online guide for VSCode][vscode] helps with this.

# VSCode
## Installation
* The [online guide][vscode] was very helpful.

## Usage
* Had issues with interface. Fixed by restarting.

# Git

# Julia
The following is executed in the terminal.

Download the zipped julia program.
```
wget https://julialang-s3.julialang.org/bin/linux/aarch64/1.5/julia-1.5.3-linux-aarch64.tar.gz
```

Unzip the zip folder
```
tar -xvzf julia-1.5.3-linux-aarch64.tar.gz
```

Copy the unzipped julia folder to `/opt/`
```
sudo cp -r julia-1.5.3 /opt/
```

Create a symbolic link so `julia` can be called from the terminal.
```
sudo ln -s /opt/julia-1.5.3/bin/julia /usr/local/bin/julia
``` 

# LaTeX
Installation was easy. In the terminal:
```
sudo apt-get install texlive-full
```

---

[vscode]: https://code.visualstudio.com/blogs/2020/12/03/chromebook-get-started