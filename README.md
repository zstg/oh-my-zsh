# oh-my-zsh setup

## Get Oh-My-Zsh first
```bash
sh -c "$(wget https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh -O -)"
```
## Clone this repo
<!-- ```bash

cd /tmp && git clone https://github.com/zstg/oh-my-zsh 
rm -rf $HOME/**zsh**
 mv ./oh-my-zsh/** $HOME
mv ~/zshrc ~/.zshrc && mv ~/zshenv ~/.zshenv
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
echo plugins=(zsh-syntax-highlighting) >> ~/.zshrc
```
-->

```bash
if [-f "~/.zshrc" ];
 echo Moving your already existing ~/.zshrc to ~/.zshrc_bak ...
 mv ~/.zshrc ~/.zshrc.bak 
fi
wget https://raw.githubusercontent.com/zstg/oh-my-zsh/main/zshrc -O ~/.zshrc
wget https://raw.githubusercontent.com/zstg/oh-my-zsh/main/zshenv -O ~/.zshenv
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
echo 'plugins=(zsh-syntax-highlighting)' >> ~/.zshrc
echo source ~/.oh-my-zsh/custom/plugins/zsh-syntax-highlighting/zsh-syntax-highlighting.plugin.zsh >> ~/.zshrc
```
## Next time you `exec zsh` the plugin will automatically get installed.
