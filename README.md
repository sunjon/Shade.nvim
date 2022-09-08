**This is a fork with all the existing PRs merged and a number of additional fixes. I will try to further improve the plugin in the future.** -> use tint.nvim instead

# shade.nvim

Shade is a Neovim plugin that dims your inactive windows, making it easier to see the active window at a glance.

<img src="https://raw.githubusercontent.com/sunjon/images/master/shade_demo.gif" alt="screenshot" width="800"/>

## Installation

### [Packer](https://github.com/wbthomason/packer.nvim) 

```
use 'jghauser/shade.nvim'
```
### [Vim-Plug](https://github.com/junegunn/vim-plug)

```
Plug 'jghauser/shade.nvim'
```

## Configuration

```
require'shade'.setup({
  overlay_opacity = 50,
  opacity_step = 1,
  keys = {
    brightness_up    = '<C-Up>',
    brightness_down  = '<C-Down>',
    toggle           = '<Leader>s',
  },
  exclude_filetypes = { "neo-tree", "markdown" }
})
```

* The `keys` table above shows available actions. No mappings are defined by default.

* The color of the numbers in the brightness control popup can be customized by creating a highlight group named: `ShadeBrightnessPopup` and setting the attributes to your liking.

* The `exclude_filetypes` table above is just an example. No filetypes are excluded by default.

## Interactions with other plugins

Other plugins with floating windows (for example `treesitter-context`) might have these not show up. This can be fixed by setting the `zindex` to 50.

## License

Copyright (c) the authors. Distributed under the MIT license

