# linuxify

Transparently transform the macOS CLI into a fresh GNU/Linux CLI experience by

- installing missing GNU programs
- updating outdated GNU programs
- replacing pre-installed BSD programs with their preferred GNU implementation
- installing other programs common among popular GNU/Linux distributions

## Install

```bash
curl https://raw.githubusercontent.com/fabiomaia/linuxify/master/linuxify > $HOME/.linuxify
. ~/.linuxify
linuxify
```

Source the script from your shell's rc file:

```bash
source $HOME/.linuxify
```

Call the `linuxify_install` function.

## Uninstall

Call the `linuxify_uninstall` and unsource the script from your shell.

```bash
linuxify uninstall
sed -i '/source $HOME/.linuxify/d' ~/.bashrc
sed -i '/source $HOME/.linuxify/d' ~/.zshrc
```
