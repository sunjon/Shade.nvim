# shade.nvim

Shade is a Neovim plugin that dims your inactive windows, making it easier to see the active window at a glance.

<img src="https://raw.githubusercontent.com/sunjon/images/master/shade_demo.gif" alt="screenshot" width="800"/>

## Installation

### [Packer.nvim](https://github.com/wbthomason/packer.nvim) 

```
use 'sunjon/shade.nvim'
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
  }
})
```

* The `keys` table above shows available actions. No mappings are defined by default.


## License

Copyright (c) Senghan Bright. Distributed under the MIT license

