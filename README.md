[![Add to Cursor](https://fastmcp.me/badges/cursor_dark.svg)](https://fastmcp.me/MCP/Details/1825/android-project-mcp-server)
[![Add to VS Code](https://fastmcp.me/badges/vscode_dark.svg)](https://fastmcp.me/MCP/Details/1825/android-project-mcp-server)
[![Add to Claude](https://fastmcp.me/badges/claude_dark.svg)](https://fastmcp.me/MCP/Details/1825/android-project-mcp-server)
[![Add to ChatGPT](https://fastmcp.me/badges/chatgpt_dark.svg)](https://fastmcp.me/MCP/Details/1825/android-project-mcp-server)
[![Add to Codex](https://fastmcp.me/badges/codex_dark.svg)](https://fastmcp.me/MCP/Details/1825/android-project-mcp-server)
[![Add to Gemini](https://fastmcp.me/badges/gemini_dark.svg)](https://fastmcp.me/MCP/Details/1825/android-project-mcp-server)

# Android Project MCP Server

A Model Context Protocol server that builds Android project that enables seamless workflow working with Android projects in Visual Studio Code using extensions like Cline or Roo Code.

<a href="https://glama.ai/mcp/servers/@ShenghaiWang/androidbuild">
  <img width="380" height="200" src="https://glama.ai/mcp/servers/@ShenghaiWang/androidbuild/badge" alt="Android Project Server MCP server" />
</a>

### Available Tools

- `build` - Build Android project
    - `folder` (string, required): The full path of the current folder that the Android project sits
- `test` - Run unit test
    - `folder` (string, required): The full path of the current folder that the Android project sits
- `instrumentedTest` - Run Instrumented test
  - `folder` (string, required): The full path of the current folder that the Android project sits

## Installation


### Using uv (recommended)

When using [`uv`](https://docs.astral.sh/uv/) no specific installation is needed. We will
use [`uvx`](https://docs.astral.sh/uv/guides/tools/) to directly run *mcpandroidbuild*.

### Using PIP

Alternatively you can install `mcpandroidbuild` via pip:

```
pip install mcpandroidbuild
```

After installation, you can run it as a script using:

```
python -m  mcpandroidbuild
```

## Configuration

### Configure for Claude.app

Add to your Claude settings:

<details>
<summary>Using uvx</summary>

```json
"mcpServers": {
  "mcpandroidbuild": {
    "command": "uvx",
    "args": ["mcpandroidbuild"]
  }
}
```
</details>

<details>
<summary>Using pip installation</summary>

```json
"mcpServers": {
  "mcpandroidbuild": {
    "command": "python",
    "args": ["-m", "mcpandroidbuild"]
  }
}
```
</details>


## License

mcpandroidbuild MCP tool is licensed under the MIT License. This means you are free to use, modify, and distribute the software, subject to the terms and conditions of the MIT License. For more details, please see the LICENSE file in the project repository.