MCP Server Demo

This is a demo Model Context Protocol (MCP)
 server that integrates with Claude Desktop. It shows how to set up and run a custom MCP server.

🚀 Getting Started
1. Clone the Repository
git clone https://github.com/your-username/mcp-server-demo.git
cd mcp-server-demo

2. Install Dependencies

You can use either uv or pip to install dependencies.

Using uv (recommended)
uv add "mcp[cli]"

Using pip
pip install "mcp[cli]"

3. Install the MCP Server

Run the following to install your server into Claude Desktop:

uv run mcp install main.py


You should see logs like:

[INFO] Added server 'Demo' to Claude config
[INFO] Successfully installed Demo in Claude app

🛠 Using in Claude Desktop

Open Claude Desktop.

Go to Settings → Developer → Edit Config and confirm the Demo server entry exists.

Restart Claude Desktop.

In the chat window, click the hammer icon (🛠️) to see available MCP tools from this server.

Start interacting with your Demo MCP server.

🔍 Troubleshooting

If the server does not appear in Claude:

Ensure uv run mcp install main.py ran without errors.

Restart Claude Desktop.

Check the Claude logs for MCP errors:

Windows: %APPDATA%\Claude\logs\

macOS: ~/Library/Logs/Claude/