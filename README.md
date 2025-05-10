# Cursor Version Manager

A shell script to manage multiple versions of [Cursor](https://www.cursor.com/) locally on your machine. **Built for linux users that use the AppImage distribution of Cursor.**

### Installation

#### Option 1: Install system-wide

```bash
sudo curl -L -o /usr/local/bin/cvm https://github.com/ivstiv/cursor-version-manager/releases/download/1.4.0/cvm.sh
sudo chmod +x /usr/local/bin/cvm
```

#### Option 2: Use it as a local script

```bash
curl -L -o cvm.sh https://github.com/ivstiv/cursor-version-manager/releases/download/1.4.0/cvm.sh
chmod +x cvm.sh
```

#### Download cursor and add an alias to it
```bash
# system-wide
cvm --install
# local script
./cvm.sh --install
```

### Usage
```
cvm.sh — Cursor version manager

Examples:
  ./cvm.sh --version
  sh cvm.sh --list-local
  bash cvm.sh --use 0.40.4

Notice*:
  The AppImage files are downloaded from the official Cursor releases.
  The list of download sources can be found at https://github.com/oslook/cursor-ai-downloads

Options:
  --list-local         Lists locally available versions
  --list-remote        Lists versions available for download
  --download <version> Downloads a version
  --update             Downloads and selects the latest version
  --use <version>      Selects a locally available version
  --active             Shows the currently selected version
  --remove <version>   Removes a locally available version
  --install            Adds an alias `cursor` and downloads the latest version
  --uninstall          Removes the Cursor version manager directory and alias
  --update-script      Updates the (cvm.sh) script to the latest version
  -v --version         Shows the current and latest versions for cvm.sh and Cursor
  -h --help            Shows this message
```