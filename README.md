# pubspec-assist.nvim

A clone of a neovim clone of [pubspec-assist](https://github.com/jeroen-meijer/pubspec-assist) a plugin for adding and updating dart dependencies in pubspec.yaml files.

<img width="827" alt="Screen Shot 2022-03-20 at 21 24 28" src="https://user-images.githubusercontent.com/22454918/159186795-c26bd9e8-2476-430a-8c97-b051b1f9648e.png">

## Features

Version picker (using `vim.ui.select`)

<img width="959" alt="Screen Shot 2022-03-20 at 21 24 45" src="https://user-images.githubusercontent.com/22454918/159186794-666a29f3-8668-4eae-b0d7-8384b4e7d9b8.png">

Package search (using `vim.ui.input`)

<img width="659" alt="Screen Shot 2022-03-20 at 21 34 18" src="https://user-images.githubusercontent.com/22454918/159186904-3a1a11e6-3c46-44ab-8ba3-a747eeb5eddf.png">

## Status:

This plugin is in _alpha_ but should be stable enough for daily usage.

## Requirements:

- `nvim 0.7+`
- `plenary.nvim`

## Installation

```lua
use {
  'RyanCarrier/pubspec-assist.nvim',
  requires = 'plenary.nvim',
  config = function()
    require('pubspec-assist').setup()
  end,
}
```

## Usage

```lua
  -- Jump to the latest version
  vim.keymap.set("n", "<leader>pal", function() pa.set_latest_version() end);
  -- Show the version picker
  vim.keymap.set("n", "<leader>pap", function() pa.open_version_picker() end);
```

## Contributing

Send PR or don't use
