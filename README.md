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

## Installing Neovim itself (no sudo / no FUSE)

On a login node without root or FUSE support (AppImages fail with
`dlopen(): error loading libfuse.so.2`), install the plain binary tarball
instead:

```bash
mkdir -p ~/bin
cd ~/bin
curl -L https://github.com/neovim/neovim/releases/download/v0.10.0/nvim-linux64.tar.gz -o nvim.tar.gz
tar xzf nvim.tar.gz
ln -sf nvim-linux64/bin/nvim nvim
```

Add `~/bin` to your `PATH`. If your login shell is `csh`/`tcsh` (not bash),
add this to `~/.cshrc` instead of `~/.bashrc`:

```csh
if ($?PATH) then
  setenv PATH "$HOME/bin:$PATH"
else
  setenv PATH "$HOME/bin"
endif
```

Then log out and back in, and confirm with `nvim --version`.

Then clone this config:

```bash
git clone https://github.com/rishisinhanj/nvim-config ~/.config/nvim
nvim
```
