# user-config

## install software with brew

```sh
# homebrew
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
#cd ~
#mkdir homebrew && curl -L https://github.com/Homebrew/brew/tarball/master | tar xz --strip-components 1 -C homebrew
#eval "$(homebrew/bin/brew shellenv)"
#brew analytics off
#brew update --force --quiet
#chmod -R go-w "$(brew --prefix)/share/zsh"
#echo 'eval "$(homebrew/bin/brew shellenv)"' >> ~/.zshrc

# oh-my-zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

brew install zsh-syntax-highlighting
echo "source $(brew --prefix)/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh" >> ~/.zshrc

brew install zsh-autosuggestions
echo "source $(brew --prefix)/share/zsh-autosuggestions/zsh-autosuggestions.zsh" >> ~/.zshrc

#brew install fish # for minimal setups

# dev
brew install 5ire beekeeper-studio ffmpeg ghostty github grandperspective lm-studio

# container
brew install cubectl docker-compose kubernetes-cli podman podman-desktop

# personal
brew install obs tailscale vlc

# hardware
brew install linearmouse

# browser
brew install google-chrome # arc zen-browser

# ide
brew install cursor visual-studio-code # zed

# google dev
brew install flutter google-cloud-sdk google-drive
flutter --disable-analytics

# python
brew install uv

# nodejs
brew install nvm # asdf fnm volta

#echo -e "\n. $(brew --prefix asdf)/libexec/asdf.sh" >> ~/.zshrc

#echo 'eval "$(fnm env --use-on-cd)"' >> ~/.zshrc

echo 'NVM_DIR="$(brew --prefix nvm)"' >> ~/.zshrc
echo '[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm' >> ~/.zshrc
echo '[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion' >> ~/.zshrc
echo 'export NVM_DIR="$HOME/.nvm"' >> ~/.zshrc
echo 'export NODE_OPTIONS="--disable-telemetry"' >> ~/.zshrc

omz reload
nvm i node
corepack enable

# firebase dev
npm install -g firebase-cli genkit-cli

```
