# ft_count_lines.nvim

A Neovim plugin to count the total number of lines for every function in a `.c` file, ensuring compliance with 42 School's Norminette requirements.

## Features

- Parse `.c` files and display the total line count for each function.
- Helps ensure no function exceeds the maximum line count according to Norminette rules.

## Installation

To install with Lazy.nvim:

```lua
{
  "TuTaRdrgZ/ft_count_lines.nvim",
  config = function()
    require("ft_count_lines").setup({
        enable_on_start = true --Default is false
    })
  end
}
```
## Usage

Once installed and configured, the plugin will automatically analyze your .c files and provide the total line count of each function.

## Norminette Compliance

This plugin assists in verifying that the functions in your `.c` files adhere to the Norminette's function size constraints. Each function's total line count will be displayed, helping you ensure that no function exceeds the limit.

### Requirements

Neovim 0.5+ for Lua plugin support.
