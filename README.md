# .tmux.conf
Just another .tmux.conf

A clean, minimal, and productivity-focused tmux configuration designed for daily development, system administration, and offensive security workflows.

## Features

* Dual prefix support (`Ctrl-a` and `Ctrl-b`)
* Vim-style navigation and copy mode
* Mouse support with smooth scrolling
* Session persistence with automatic restore
* Smart pane splitting (retains working directory)
* Fast pane switching (with and without prefix)
* Clean and minimal status bar
* Clipboard integration (works over SSH)

## Key Bindings

| Action               | Key                  |   |
| -------------------- | -------------------- | - |
| Prefix               | `Ctrl-a` or `Ctrl-b` |   |
| Split Vertical       | `                    | ` |
| Split Horizontal     | `-`                  |   |
| Navigate Panes       | `h j k l`            |   |
| Navigate (no prefix) | `Alt + h/j/k/l`      |   |
| Resize Panes         | `Shift + H/J/K/L`    |   |
| Reload Config        | `Prefix + r`         |   |
| Sync Panes           | `Prefix + S`         |   |

## Plugins

Managed via TPM:

* tmux-sensible
* tmux-yank
* tmux-resurrect
* tmux-continuum
* tmux-better-mouse-mode

## Installation

```bash
curl -o ~/.tmux.conf https://raw.githubusercontent.com/ndeepak/.tmux.conf/refs/heads/main/.tmux.conf
```

(Optional) If you keep configs in a directory:
```bash
mkdir -p ~/.tmux
ln -s ~/.tmux/.tmux.conf ~/.tmux.conf
```

### Plugin Setup (TPM)
Clone TPM manually:
```bash
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```
Then inside tmux:

```bash
Prefix + I
# OR
Ctrl-a + I
```

## Notes

* Designed for speed and minimal friction
* Works well over SSH and remote environments
* Optimized for terminal-based workflows (Vim, pentesting, DevOps)

---

Maintained by Deepak Nagarkoti [@ndeepak](https://github.com.ndeepak)
