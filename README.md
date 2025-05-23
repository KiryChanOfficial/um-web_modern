# TIPS  
**此仓库是由于无法Fork而重新建立的仓库，并非官方仓库**  
**原始仓库在这 https://git.unlock-music.dev/um/cli**    

> **WARNING**  
> 如无必要请勿 Fork 该仓库。  

  ---  

# Unlock Music Project - CLI Edition

Original: Web Edition https://git.unlock-music.dev/um/web

- [![Build Status](https://ci.unlock-music.dev/api/badges/um/cli/status.svg)](https://ci.unlock-music.dev/um/cli)
- [Release Download](https://git.unlock-music.dev/um/cli/releases/latest)
- [Latest Build](https://git.unlock-music.dev/um/-/packages/generic/cli-build/)

## Features

- [x] All Algorithm Supported By `unlock-music/web`
- [x] Complete Metadata & Cover Image

## Release

[Latest release](https://git.unlock-music.dev/um/cli/releases/latest).

## Install from source

- Requirements: **Golang 1.23.3**

1. run `go install unlock-music.dev/cli/cmd/um@master`

### Build from repo source

1. Pull repo source.
2. Build with `go build ./cmd/um`.

It will produce `um` or `um.exe` (Windows).

## How to use

- Drag the encrypted file to `um.exe` (Tested on Windows)
- Run: `./um [-o <output dir>] [-i] <input dir/file>`
- Use `./um -h` to show help menu

## Update CI pipeline

1. Install [Drone CI binary](https://docs.drone.io/cli/install/)
2. Edit `.drone.jsonnet`
3. Update drone CI pipeline:

   ```sh
   drone jsonnet --format --stream
   ```
