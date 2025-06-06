# user-config

## install software with brew

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# dev
brew install 5ire beekeeper-studio ghostty github grandperspective lm-studio podman-desktop

# personal
brew install obs tailscale

# browser
brew install google-chrome # arc zen-browser

# ide
brew install visual-studio-code # cursor zed

# google dev
brew install flutter google-cloud-sdk google-drive

# python
brew install uv

# nodejs
brew install nvm # asdf fnm volta

#echo -e "\n. $(brew --prefix asdf)/libexec/asdf.sh" >> ~/.zshrc

#echo 'eval "$(fnm env --use-on-cd)"' >> ~/.zshrc

echo 'export NVM_DIR="$HOME/.nvm"' >> ~/.zshrc
echo '[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm' >> ~/.zshrc
echo '[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion' >> ~/.zshrc

zsh
nvm i node
corepack enable
#pnpm install -g ...

```
