# homage-black

A Neovim port of Doom Emacs' `doom-homage-black` theme.

Near-monochrome on pure black. Keywords / functions / builtins / types are
near-white (`#DFDFDF`) and **bold**; strings / numbers are muted orange;
comments are green; everything else is plain fg. Color is used sparingly —
weight does the work.

I like to have the consistency between my emacs and nvim so I used Claude Code
shamelessly to make this port. Use this at your own risk since I will not
maintain it.

## Install

Requires Neovim 0.12+ for the built-in `vim.pack` package manager.

```lua
vim.pack.add({
  "https://github.com/bubuzzz/homage-black",
})

vim.cmd.colorscheme("homage-black")
```

Or with other managers:

```lua
-- lazy.nvim
{ "bubuzzz/homage-black" }

-- packer.nvim
use("bubuzzz/homage-black")
```

A `termguicolors`-capable terminal is required (Neovim enables this by default,
but if you've disabled it):

```lua
vim.o.termguicolors = true
```
