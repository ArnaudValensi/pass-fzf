# pass-fzf (compatible MacOS)
An extension for [pass](https://www.passwordstore.org/) that allows fuzzy
finding in the store.

requires `fzf` to be installed in the system.

require `gfind` and `gsed` to be installed in the system (`brew install findutils gnu-sed`).

# Installation
Installation is done through `pass` extensions.
```
mkdir -p $PASSWORD_STORE_DIR/.extensions/
wget https://raw.githubusercontent.com/ArnaudValensi/pass-fzf/master/fzf.bash -O $PASSWORD_STORE_DIR/.extensions/fzf.bash
chmod +x $PASSWORD_STORE_DIR/.extensions/fzf.bash
PASSWORD_STORE_ENABLE_EXTENSIONS=true pass fzf
```

# Usage
```
$ pass fzf
```
# Alias
```
$ alias passs='PASSWORD_STORE_ENABLE_EXTENSIONS=true pass fzf'
```
