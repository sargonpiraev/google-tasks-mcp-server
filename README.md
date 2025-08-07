# Google Tasks API MCP Server 🔧

![npm version](https://img.shields.io/npm/v/@sargonpiraev/google-tasks-mcp-server)
![npm downloads](https://img.shields.io/npm/dw/@sargonpiraev/google-tasks-mcp-server)
![license](https://img.shields.io/github/license/sargonpiraev/google-tasks-mcp-server)
![pipeline status](https://gitlab.com/sargonpiraev/google-tasks-mcp-server/badges/main/pipeline.svg)
![smithery badge](https://smithery.ai/badge/@sargonpiraev/google-tasks-mcp-server)
![MCP Compatible](https://img.shields.io/badge/MCP-Compatible-blue)
[![Join Discord](https://img.shields.io/discord/1331631275464671347?color=7289da&label=Discord&logo=discord)](https://discord.gg/ZsWGxRGj)

## Features

- 🔌 **Seamless AI Integration**: Direct Google Tasks API API access from Claude, Cursor, and VS Code
- 🤖 **Automated Workflows**: Automate Google Tasks API operations and data access
- 📊 **Complete API Coverage**: 14+ tools covering all major Google Tasks API features
- ⚡ **Real-time Access**: Access Google Tasks API data instantly from AI assistants
- 🔧 **Professional Integration**: Error handling, validation, and comprehensive logging

## Get Your Credentials

Before installation, you'll need a Google Tasks API API key:

1. Open Google Tasks API app or web interface
2. Go to **Settings → Account → API Access**
3. Generate new API key or copy existing one
4. Save this key for the installation steps below

## Requirements

- Node.js >= v18.0.0
- Google Tasks API API key
- Cursor, VS Code, Claude Desktop or another MCP Client

## Installation

<details>
<summary><b>Installing via Smithery</b></summary>

To install Google Tasks API MCP Server for any client automatically via [Smithery](https://smithery.ai):

```bash
npx -y @smithery/cli@latest install @sargonpiraev/google-tasks-mcp-server --client <CLIENT_NAME>
```

</details>

<details>
<summary><b>Install in Cursor</b></summary>

#### Cursor One-Click Installation

[![Install MCP Server](https://cursor.com/deeplink/mcp-install-dark.svg)](https://cursor.com/install-mcp?name=@sargonpiraev/google-tasks-mcp-server&config=eyJjb21tYW5kIjoibnB4IiwiYXJncyI6WyIteSIsIkBzYXJnb25waXJhZXYvZ29vZ2xlLXRhc2tzLW1jcC1zZXJ2ZXIiXSwiZW52Ijp7IkdPT0dMRV9UQVNLU19DTElFTlRfSUQiOiJ5b3VyX2dvb2dsZV90YXNrc19jbGllbnRfaWRfaGVyZSIsIkdPT0dMRV9UQVNLU19DTElFTlRfU0VDUkVUIjoieW91cl9nb29nbGVfdGFza3NfY2xpZW50X3NlY3JldF9oZXJlIn19)

#### Manual Configuration

Add to your Cursor `~/.cursor/mcp.json` file:

```json
{
  "mcpServers": {
    "google-tasks-mcp-server": {
      "command": "npx",
      "args": ["-y", "@sargonpiraev/google-tasks-mcp-server"],
      "env": {
        "GOOGLE_TASKS_CLIENT_ID": "your-google_tasks_client_id",
        "GOOGLE_TASKS_CLIENT_SECRET": "your-google_tasks_client_secret"
      }
    }
  }
}
```

</details>

<details>
<summary><b>Install in VS Code</b></summary>

[![Install in VS Code](https://img.shields.io/badge/VS_Code-Install_MCP-0098FF)](vscode:mcp/install?%7B%22name%22%3A%22google-tasks-mcp-server%22%2C%22command%22%3A%22npx%22%2C%22args%22%3A%5B%22-y%22%2C%22@sargonpiraev/google-tasks-mcp-server%22%5D%7D)

Or add manually to your VS Code settings:

```json
"mcp": {
  "servers": {
    "google-tasks-mcp-server": {
      "type": "stdio",
      "command": "npx",
      "args": ["-y", "@sargonpiraev/google-tasks-mcp-server"],
      "env": {
        "GOOGLE_TASKS_CLIENT_ID": "your-google_tasks_client_id",
        "GOOGLE_TASKS_CLIENT_SECRET": "your-google_tasks_client_secret"
      }
    }
  }
}
```

</details>

<details>
<summary><b>Install in Claude Desktop</b></summary>

Add to your `claude_desktop_config.json`:

```json
{
  "mcpServers": {
    "google-tasks-mcp-server": {
      "command": "npx",
      "args": ["-y", "@sargonpiraev/google-tasks-mcp-server"],
      "env": {
        "GOOGLE_TASKS_CLIENT_ID": "your-google_tasks_client_id",
        "GOOGLE_TASKS_CLIENT_SECRET": "your-google_tasks_client_secret"
      }
    }
  }
}
```

</details>

## Available Tools

- **`list-task-lists`**: List task lists
- **`insert-task-list`**: Create task list
- **`get-task-list`**: Get task list
- **`update-task-list`**: Update task list
- **`patch-task-list`**: Patch task list
- **`delete-task-list`**: Delete task list
- **`list-tasks`**: List tasks
- **`insert-task`**: Create task
- **`get-task`**: Get task
- **`update-task`**: Update task
- **`patch-task`**: Patch task
- **`delete-task`**: Delete task
- **`move-task`**: Move task
- **`clear-tasks`**: Clear completed tasks

**Total: 14 tools available** 🎯

## Support This Project

Hi! I'm Sargon, a software engineer passionate about AI tools and automation. I create open-source MCP servers to help developers integrate AI assistants with their favorite services.

Your support helps me continue developing and maintaining these tools, and motivates me to create new integrations that make AI assistants even more powerful! 🚀

[![Support on Boosty](https://img.shields.io/badge/Support-Boosty-orange?logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggZD0iTTEyIDJMMTMuMDkgOC4yNkwyMCA5TDEzLjA5IDE1Ljc0TDEyIDIyTDEwLjkxIDE1Ljc0TDQgOUwxMC45MSA4LjI2TDEyIDJaIiBmaWxsPSJ3aGl0ZSIvPgo8L3N2Zz4K)](https://boosty.to/sargonpiraev)

## Connect with Author

- 🌐 Visit [sargonpiraev.com](https://sargonpiraev.com)
- 📧 Email: [sargonpiraev@gmail.com](mailto:sargonpiraev@gmail.com)
- 💬 Join [Discord](https://discord.gg/ZsWGxRGj)
