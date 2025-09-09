# user-config

## install software with brew

```sh
# ensure default identity
ssh-keygen

# homebrew
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
eval "$(/opt/homebrew/bin/brew shellenv)"
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zshrc

#cd ~
#mkdir homebrew && curl -L https://github.com/Homebrew/brew/tarball/master | tar xz --strip-components 1 -C homebrew
#eval "$(homebrew/bin/brew shellenv)"
brew analytics off
#brew update --force --quiet
chmod -R go-w "$(brew --prefix)/share/zsh"
# echo 'eval "$(homebrew/bin/brew shellenv)"' >> ~/.zshrc

# oh-my-zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

brew install zsh-syntax-highlighting
echo "source $(brew --prefix)/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh" >> ~/.zshrc

brew install zsh-autosuggestions
echo "source $(brew --prefix)/share/zsh-autosuggestions/zsh-autosuggestions.zsh" >> ~/.zshrc

#brew install fish # for minimal setups

# dev
brew install cmake ffmpeg fzf rga pandoc poppler
brew install beekeeper-studio ghostty github grandperspective

# llms
brew install 5ire lm-studio ollama-app

# docker
brew install docker-compose helm kubernetes-cli kubernetes-cli podman podman-desktop

# media
brew install losslesscut obs vlc

# vpn
brew install surfshark tailscale-app

# hardware
brew install linearmouse

# browser
brew install google-chrome thebrowsercompany-dia # zen-browser

# ide
brew install cursor visual-studio-code # zed

echo 'export EDITOR="code --wait"' >> ~/.zshrc
echo 'export VISUAL="code --wait"' >> ~/.zshrc

# google
brew install flutter google-cloud-sdk google-drive
flutter --disable-analytics

# python
brew install miniconda uv

# nodejs
brew install nvm # asdf fnm volta

#echo -e "\n. $(brew --prefix asdf)/libexec/asdf.sh" >> ~/.zshrc

#echo 'eval "$(fnm env --use-on-cd)"' >> ~/.zshrc

brew tap oven-sh/bun
brew install bun

echo 'NVM_DIR="$(brew --prefix nvm)"' >> ~/.zshrc
echo '[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm' >> ~/.zshrc
echo '[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion' >> ~/.zshrc
echo 'export NVM_DIR="$HOME/.nvm"' >> ~/.zshrc

omz reload
nvm i node
corepack enable
echo 'nvm use 24' >> ~/.zshrc

npm i -g bun opencode-ai # npm

# google
npm i -g firebase-cli genkit-cli @google/gemini-cli
```

