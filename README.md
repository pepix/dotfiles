# dotfiles

## How to set up

### Prerequisites

- Use `zsh` as your shell.
- Install `oh-my-zsh` and make sure `git` plugin is enabled.

### 1. Clone the repository

Clone the repository to your root directory.

```bash
$ git clone https://github.com/pepix/dotfiles.git
```

### 2. Create symlinks

Run below commands under root directory.

```bash
$ ln -s dotfiles/.vimrc .vimrc
$ ln -s dotfiles/.zsh_custom .zsh_custom
```

### 3. Add custom commands to `.zshrc`

Add below script to your `.zshrc`.

```bash
if [ -f ~/.zsh_custom ]; then
    source ~/.zsh_custom
fi
```

### 4. Reload `.zshrc`

```bash
$ source ~/.zshrc
```
