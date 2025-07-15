# MCP PowerShell Exec Server

## Overview
MCP PowerShell Exec Server is a lightweight server that accepts PowerShell scripts as strings, executes them, and returns the output. Enabling AI assistants to understand and work with PowerShell.

## Features
- Accepts PowerShell scripts via string input
- Executes scripts securely in an MCP Server environment
- Returns execution results in real-time

## Installation
Clone the repository and set up the server:

```powershell
git clone https://github.com/yourusername/mcp-powershell-exec.git
cd mcp-powershell-exec
```
## In Action

Watch the video to see MCP PowerShell Exec Server in action:

<a href="https://youtu.be/XmYaCJ0bNsE"><img src="https://img.youtube.com/vi/XmYaCJ0bNsE/0.jpg" width="600"/></a>

## Usage

### Integration with GitHub Copilot in VSCode Insiders

To use this MCP server with GitHub Copilot in VSCode Insiders, follow these steps:

1. **Install VSCode Insiders**
   - Download and install the latest version of [VSCode Insiders](https://code.visualstudio.com/insiders/)

1. **Install GitHub Copilot Extension**
   - Open VSCode Insiders
   - Go to the Extensions marketplace
   - Search for and install "GitHub Copilot"

3. **Configure MCP Server**
   - Open .vscode/mcp.json
   ```json
   {
    "servers": {
        "powershell-integration": {
            "command": "py", // Python executable
            "args": [
               "drive:/yourpath/server.py"
            ],
            "env": {}
        }
    }
   }
   ```
   Replace the path with the actual path to your `server.py` file.
   

1. **Enable Agent Mode**
   - Open Copilot chat in VSCode Insiders
   - Click on "Copilot Edits"
   - Choose "Agent mode"
   - Click the refresh button in the chat input to load the available tools

## System Requirements

- **Python**: Version 3.10 or higher (required for optimal performance)
- **PowerShell**: Version 5.1 

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support

For issues and questions:
- Create an issue in this GitHub repository   
