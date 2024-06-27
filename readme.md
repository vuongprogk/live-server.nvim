# live-server.nvim

Live reload HTML, CSS, and JavaScript files inside neovim with the power of
[live-server](https://www.npmjs.com/package/live-server).

## Installation

1. Install [live-server](https://www.npmjs.com/package/live-server) globally
   with your node.js package manager of choice.

2. Install regularly with your neovim package manager

For example, a config with [npm](https://www.npmjs.com) and
[lazy.nvim](https://github.com/folke/lazy.nvim) may look like the following:

```lua
require('lazy').setup {
    {
        'vuongprogk/live-server.nvim',
        build = 'npm install -g live-server',
        cmd = { 'LiveServerStart', 'LiveServerStop' },
        config = true
    }
}
```

## Configuration

Configure via the setup function (or use the defaults with no arguments):

```lua
require('live-server').setup(opts)
```

See `:h live-server` for more information

## Usage

`:LiveServerStart`: start the live server

`:LiveServerStop`: stop the live server

## Acknowledgements

1. [barrett-ruth/live-server.nvim](https://github.com/barrett-ruth/live-server.nvim): I folk from it! 
