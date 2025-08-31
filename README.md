# MCP Server Demo

[![Python](https://img.shields.io/badge/python-3.10%2B-blue.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![MCP](https://img.shields.io/badge/MCP-Supported-purple.svg)](https://modelcontextprotocol.io)
[![Claude](https://img.shields.io/badge/Claude-Desktop-orange.svg)](https://claude.ai)

## Key Features and Highlights
- Python based server demo

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/mcp-server-demo.git
    ```
2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## 2. Install Dependencies

You can use either uv or pip to install dependencies.
```bash
Using uv (recommended)
uv add "mcp[cli]"
```

```bash
Using pip
pip install "mcp[cli]"
```


## 3. Install the MCP Server


Run the following to install your server into Claude Desktop:

```bash
uv run mcp install main.py
```

You should see logs like:

[INFO] Added server 'Demo' to Claude config
[INFO] Successfully installed Demo in Claude app


## 🛠 Using in Claude Desktop

```bash
1. Open Claude Desktop  
2. Go to Settings → Developer → Edit Config and confirm the `Demo` server entry exists  
3. Restart Claude Desktop  
4. In the chat window, click the hammer icon (🛠️) to see available MCP tools from this server  
5. Start interacting with your Demo MCP server 🎉  
```


## 🔍 Troubleshooting

If the server does not appear in Claude:
```bash
- Ensure `uv run mcp install main.py` ran without errors
```

- Restart Claude Desktop 

```bash
- Check Claude logs for MCP errors:  
    • Windows: %APPDATA%\Claude\logs\  
    • macOS:   ~/Library/Logs/Claude/  
```

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.







