# oh-my-zsh setup

## Get Oh-My-Zsh first
```bash
sh -c "$(wget https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh -O -)"
```
## Clone this repo
```bash

cd /tmp && git clone https://github.com/zstg/oh-my-zsh 
rm -rf $HOME/**zsh**
mv ./oh-my-zsh/.zsh** $HOME
```

## Next time you `exec zsh` the plugin will automatically get installed.
