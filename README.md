# Neovim Config

A minimal, beginner-friendly Neovim configuration with:
- **Telescope**: Fuzzy file finder (`<leader>ff`)
- **Treesitter**: Syntax highlighting
- **LSP**: Language server support (optional)
- **Completion**: Auto-completion with nvim-cmp
- **File Explorer**: nvim-tree (`<leader>e`)
- **Theme**: Tokyo Night

## Installation

```bash
git clone https://github.com/rishisinhanj/nvim-config ~/.config/nvim
nvim
```

Plugins will auto-install on first launch via lazy.nvim.

## Keybindings

| Key | Action |
|-----|--------|
| `<leader>ff` | Find files |
| `<leader>fg` | Live grep (search) |
| `<leader>fb` | Buffers |
| `<leader>e` | Toggle file explorer |
| `<leader>w` | Save |
| `<leader>q` | Quit |

## Requirements

- Neovim 0.8+
- Git
- ripgrep (for live_grep)
