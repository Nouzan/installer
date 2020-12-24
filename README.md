# Installer

Install all the tools of what I need.

## Steps

### Install Rust toolchans

```sh
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

### (Optional) Use mirror

```sh
echo "RUSTUP_DIST_SERVER=https://mirrors.tuna.tsinghua.edu.cn/rustup"  >> ~./ .cargo/env
```

### Install some tools by Cargo

```sh
cargo install bottom ripgrep bat starship
```

#### Setup Starship


1. If I use `bash`, add the following to the end of `~/.bashrc`:

```sh
# ~/.bashrc

eval "$(starship init bash)"
```

2. If I use `zsh`, add the following to the end of `~/.zshrc`:

```sh
# ~/.zshrc

eval "$(starship init zsh)"
```

### Install Emacs lastest

#### macOS

```sh
brew cask install emacs
```

#### Ubuntu

1. Add the PPA.

```sh
sudo add-apt-repository ppa:kelleyk/emacs
```

2. Install Emacs

```sh
sudo apt update
sudo apt install emacs27
```
