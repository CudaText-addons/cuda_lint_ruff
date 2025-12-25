Linter for CudaLint plugin.
It adds support for Python lexer.
It uses 'Ruff'.

'Ruff' is an extremely fast Python linter and code formatter:
https://github.com/astral-sh/ruff
'Ruff' must be in your system PATH or in the Ruff folder (portable use) inside CudaText directory.

For example, to install it on Windows, download ruff.exe from GitHub releases and place it in Ruff folder inside CudaText directory.
On Linux: curl -LsSf https://astral.sh/ruff/install.sh | sh
On macOS: brew install ruff

Access Fix command via menu: Plugins > Ruff > Fix current file
Access Format command via menu: Plugins > Ruff > Format current file
Edit configuration file via menu: Plugins > Ruff > Config
Show help via menu: Plugins > Ruff > Help

To customize rules, create settings/ruff_config.json with:
{
  "ignore": [
    "E501",
    "W191"
  ],
  "select": [
    "E",
    "W",
    "F",
    "B",
    "I"
  ]
}

Ruff automatically reads pyproject.toml or ruff.toml from your project directory.
Plugin select/ignore settings take precedence over project configuration.

Author: Bruno Eduardo

License: MIT
