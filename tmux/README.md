# tmux Configuration

This repository contains a custom `tmux.conf` file.

## Installation

To use this configuration, copy `tmux.conf` to your tmux config directory:

```sh
mkdir -p ~/.config/tmux
cp tmux.conf ~/.config/tmux/tmux.conf
```

## Usage

After copying, restart tmux or reload the configuration:

```sh
tmux source-file ~/.config/tmux/tmux.conf
```

## Additional features

To add aliases for tmux commands, you can add the following lines to your shell configuration file (e.g., `~/.bashrc` or `~/.zshrc`):

```sh

alias tn='tmux new-session -s'
alias tl='tmux new-sessions'
alias ta='tmux attach-session'
alias tk='tmux kill-session -t'

````

After adding these aliases reload your shell configuration:

```sh
source ~/.bashrc
# or    
source ~/.zshrc
```

## Notes

- Ensure the `~/.config/tmux/` directory exists.
- This setup follows the XDG Base Directory specification.
- Adjust the configuration as needed for your workflow.