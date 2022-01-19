[![theaming.gif](https://s3.gifyu.com/images/theaming.gif)](https://gifyu.com/image/54o0)

## Installation

### Install manually

- Add the following line in `~/.config/xplr/init.lua`

  ```lua
  local home = os.getenv("HOME")
  package.path = home
  .. "/.config/xplr/plugins/?/init.lua;"
  .. home
  .. "/.config/xplr/plugins/?.lua;"
  .. package.path
  ```

- Clone the plugin

  ```bash
  mkdir -p ~/.config/xplr/plugins

  git clone https://github.com/sayanarijit/material-landscape.xplr ~/.config/xplr/plugins/material-landscape
  ```

- Require the module in `~/.config/xplr/init.lua`

  ```lua
  require("material-landscape").setup()

  # Or

  require("material-landscape").setup{
    keep_default_layout = true
  }
  ```
