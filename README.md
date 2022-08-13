# oh-my-zsh-backup
Backup of my customized oh-my-zsh configs. 

The backed-up oh-my-zsh configuration is in ***passion*** theme (with some modification on PROMPT), with plugins of ***shrink-path*** and ***zsh-autosuggestion***. 

## Install oh-my-zsh

```bash
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

## Recovering zsh configs

### Recovering custom folder

```bash
cd /path/to/oh-my-zsh-backup/
rm -rf ~/.oh-my-zsh/custom
cp -r ./.oh-my-zsh/custom ~/.oh-my-zsh/
```

### Recovering .zshrc file

```bash
cd /path/to/oh-my-zsh-backup/
mv ~/.zshrc ~/.zshrc.pre-backup
cp ./.zshrc ~/
```
Then restart the terminal to activate the changes. Enjoy! 
