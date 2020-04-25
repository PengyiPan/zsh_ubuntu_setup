Ubuntu 20.04 personal zsh setup

## Install zsh + 3 plugins

```bash
sudo apt install zsh zsh-syntax-highlighting zsh-autosuggestions autojump
```

## Install config file + alias + theme

```bash
wget https://github.com/ChrisTitusTech/zsh/raw/master/.zshrc -O ~/.zshrc
mkdir -p "$HOME/.zsh"
wget https://github.com/ChrisTitusTech/zsh/raw/master/.zsh/aliasrc -O ~/.zsh/aliasrc
git clone https://github.com/sindresorhus/pure.git "$HOME/.zsh/pure"
```

## Make zsh default shell

```bash
chsh -s $(which zsh)    # May need to log out and back in to take effect
```


Reference: https://www.christitus.com/zsh/
