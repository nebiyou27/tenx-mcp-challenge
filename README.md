# Tenx MCP Challenge

A project demonstrating MCP (Model Context Protocol) configuration and AI agent integration in VS Code, following Boris Cherny principles for effective AI assistance.

## 🚀 Overview

This challenge showcases the setup of Tenx MCP integration with GitHub Copilot, enabling enhanced AI agent guidance through a feedback analytics proxy. The goal is to configure MCP servers, document the process, and verify functionality.

## 📋 Prerequisites

- **VS Code**: Latest version installed
- **GitHub Copilot**: Extension installed and authenticated
- **Environment**: Windows (configured for this setup)

## 🛠️ Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/tenx-mcp-challenge.git
cd tenx-mcp-challenge
```

### 2. Configure MCP in VS Code
1. Ensure the `.vscode/mcp.json` file exists with the following content:
   ```json
   {
     "servers": {
       "tenxfeedbackanalytics": {
         "url": "https://mcppulse.10academy.org/proxy",
         "type": "http",
         "headers": {
           "X-Device": "windows",
           "X-Coding-Tool": "vscode"
         }
       }
     },
     "inputs": []
   }
   ```

2. Reload your VS Code workspace to apply the configuration.

### 3. Verify Configuration
- Open VS Code's output panel and check for MCP-related logs.
- Confirm the proxy server is reachable (expect "Connection state: Running" in logs).
- Test by running a query that triggers feedback logging.

## 📁 Project Structure

```
tenx-mcp-challenge/
├── .github/
│   └── copilot-instructions.md  # AI agent rules based on Boris Cherny principles
├── .vscode/
│   └── mcp.json                 # MCP server configuration
├── FINAL_REPORT.md              # Detailed challenge completion report
└── README.md                    # This file
```

## 🎯 Key Features

- **MCP Integration**: HTTP-based proxy server for Tenx feedback analytics
- **AI Agent Guidance**: Custom instructions for GitHub Copilot behavior
- **Documentation**: Comprehensive setup and verification steps
- **Evidence-Based**: Includes logs and proof of successful connection

## 🔧 Usage

1. Open the project in VS Code.
2. Ensure MCP is configured as above.
3. Use GitHub Copilot for coding assistance - it will follow the rules in `.github/copilot-instructions.md`.
4. Monitor feedback via the Tenx proxy for analytics.

## 📊 Verification

- **Connection Proof**: Check logs for "Discovered 3 tools" and running state.
- **Functionality**: AI suggestions should align with documented principles (proactive, precise, etc.).
- **Testing**: Run sample tasks to confirm MCP server integration.

## 🤝 Contributing

This is a challenge submission. For improvements:
1. Fork the repository
2. Create a feature branch
3. Make changes and test thoroughly
4. Submit a pull request

## 📝 License

This project is for educational purposes as part of the Tenx MCP Challenge.

## 📞 Support

For issues with MCP setup, refer to the [FINAL_REPORT.md](FINAL_REPORT.md) for detailed troubleshooting.