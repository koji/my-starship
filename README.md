# my-starship

This is my starship.toml

## how to use starship.toml
https://asdf-vm.com/guide/getting-started.html

```shell
# Setup Starship prompt
if ! command -v starship &> /dev/null; then
  curl -sS https://starship.rs/install.sh | sh
fi

# Add Starship configuration to Zsh
if ! grep -q 'eval "$(starship init zsh)"' ~/.zshrc; then
  echo 'eval "$(starship init zsh)"' >> ~/.zshrc
fi

mkdir -p ~/.config
curl -o ~/.config/starship.toml https://raw.githubusercontent.com/koji/my-starship/refs/heads/main/starship.toml
```
