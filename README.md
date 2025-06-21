# Dictionary-MCP
It is a MCP using the Merriam Webster API. It can give meanings, part of speech, stems, pronunciation, more info of stems. It can be used by plugging it with claude desktop and by other ways
## How I plugged it
- I made a venv by using `virtualenv`(can use uv but was too complicated for me as I didn't know how to use it)
- Did the code of `main.py` after installing the packages
- Installing Claude Desktop and modified the config file:
```json
{
  "mcpServers": {
    "dictionary-mcp": {
      "command": "python",
      "args": ["\\main.py"],
      "cwd": "Path\\to\\mcp\\folder",
      "env": {
        "PATH": "Path\\to\\env\\Scripts;%PATH%"
      }
    }
  }
}
```
