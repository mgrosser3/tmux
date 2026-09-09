# tmux config

My personal `tmux` configuration.

## Features

- **Prefix**: `Ctrl+Space` instead of `Ctrl+b`
- **Mouse support** enabled
- **Vim-style pane navigation**: `h`/`j`/`k`/`l` to move between panes
- **Split panes**: `v` (horizontal), `V` (vertical) — opens in the current path
- **Resize panes**: `arrow keys` (repeatable, `-r`)
- **Clipboard integration** via `set-clipboard` and `allow-passthrough`
- **Theme**: [rose-pine/tmux](https://github.com/rose-pine/tmux) (`moon` variant) with a customized status bar (host, user, directory, date/time)
- **No escape delay** (`escape-time 0`)
- Plugin management via [TPM](https://github.com/tmux-plugins/tpm)

## Installation

1. Clone this repo to `~/.config/tmux`:

   ```sh
   git clone https://github.com/mgrosser3/tmux ~/.config/tmux
   ```

2. Install [TPM](https://github.com/tmux-plugins/tpm), if not already installed:

   ```sh
   git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
   ```

3. Start tmux and install plugins with `prefix + I` (capital i).

## Reloading the config

Inside a running tmux session:

```sh
tmux source-file ~/.config/tmux/tmux.conf
```

## License

MIT, see [LICENSE](LICENSE).
