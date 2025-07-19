# 10 Microsoft MCP Servers from Microsoft DevBlogs

Based on the official Microsoft DevBlogs article, here are the 10 Microsoft MCP servers designed to accelerate development workflows:

## 1. 📚 Microsoft Learn Docs MCP Server

**Purpose**: Cloud-hosted service providing real-time access to official Microsoft documentation[1]

**Key Features**:
- Connects to `https://learn.microsoft.com/api/mcp`[1]
- Semantic search across Microsoft Learn, Azure documentation, and Microsoft 365 sources[1]
- Returns up to 10 high-quality content chunks with article titles and URLs[1]
- Always accesses the latest Microsoft documentation as published[1]

**Use Cases**: Finding az CLI commands, configuring Entity Framework with dependency injection, reviewing code against Microsoft performance recommendations[1]

## 2. ☁️ Azure MCP Server

**Purpose**: Comprehensive suite of 15+ specialized Azure service connectors[1]

**Key Modules**:
- **Database Connectors**: Direct natural language access to Azure Database for PostgreSQL and SQL Server[1]
- **Azure Monitor**: KQL-powered log analysis and operational insights[1]
- **Resource Management**: Full Azure resource lifecycle management[1]
- **Authentication**: DefaultAzureCredential and managed identity patterns[1]
- **Storage Services**: Blob Storage, Queue Storage, and Table Storage operations[1]
- **Container Services**: Azure Container Apps, Container Instances, and AKS management[1]

**Benefits**: Improves code quality by providing Azure code that follows recommended patterns for production workloads[1]

## 3. 🐙 GitHub MCP Server

**Purpose**: Official GitHub MCP Server providing seamless integration with GitHub's entire ecosystem[1]

**Key Capabilities**:
- **GitHub Actions**: Complete CI/CD pipeline management, workflow monitoring, and artifact handling[1]
- **Pull Requests**: Create, review, merge, and manage PRs with comprehensive status tracking[1]
- **Issues**: Full issue lifecycle management, commenting, labeling, and assignment[1]
- **Security**: Code scanning alerts, secret detection, and Dependabot integration[1]
- **Notifications**: Smart notification management and repository subscription control[1]

**Authentication Options**: Supports both OAuth and Personal Access Tokens, with configurable toolsets[1]

## 4. 🔄 Azure DevOps MCP Server

**Purpose**: Connects to Azure DevOps services for comprehensive project management[1]

**Capabilities**:
- Work item tracking and management[1]
- Build pipeline management[1]
- Repository operations[1]
- Sprint and project management tasks[1]

**Use Cases**: Managing work items, checking build statuses, querying repositories, and handling project management tasks directly from AI assistant[1]

## 5. 📝 MarkItDown MCP Server

**Purpose**: Comprehensive document conversion server that transforms various file formats into high-quality Markdown[1]

**Supported Formats**:
- **Office Documents**: PDF, PowerPoint (PPTX), Word (DOCX), Excel (XLSX/XLS)[1]
- **Media Files**: Images (with EXIF metadata and OCR), Audio (with EXIF metadata and speech transcription)[1]
- **Web Content**: HTML, RSS feeds, YouTube URLs, Wikipedia pages[1]
- **Data Formats**: CSV, JSON, XML, ZIP files[1]
- **Publishing Formats**: EPub, Jupyter notebooks (.ipynb)[1]

**Advanced Features**: LLM-powered image descriptions, Azure Document Intelligence integration, audio transcription[1]

## 6. 🗃️ SQL Server MCP Server

**Purpose**: Provides conversational access to SQL Server databases (on-premises, Azure SQL, or Fabric)[1]

**Benefits**: Connect with simple connection string and start querying with natural language[1]

**Use Cases**: Natural language database queries like "Find all orders that haven't been fulfilled in the last 30 days"[1]

**Setup**: Supports comprehensive database operations from schema management to data manipulation through natural language prompts[1]

## 7. 🎭 Playwright MCP Server

**Purpose**: Enables AI agents to interact with web pages for testing and automation[1]

**Key Feature**: Powers GitHub Copilot's Coding Agent with web browsing capabilities[1]

**Benefits**: Perfect for automated testing driven by natural language descriptions[1]

**Use Cases**: 
- "Test the login flow and verify that the dashboard loads correctly"[1]
- "Generate a test that searches for products and validates the results page"[1]
- Generate complete Playwright tests without access to application source code[1]

## 8. 💻 Dev Box MCP Server

**Purpose**: Manages Microsoft Dev Box environments through natural language[1]

**Benefits**: Simplifies development environment management tremendously[1]

**Use Cases**:
- "Set up a new Dev Box with the latest .NET SDK and configure it for our project"[1]
- "Check the status of all my development environments"[1]
- "Create a standardized demo environment for team presentations"[1]

**Applications**: Conference demos, team environment management, and preconfigured development environments[1]

## 9. 🤖 Azure AI Foundry MCP Server

**Purpose**: Provides comprehensive access to Azure's AI ecosystem[1]

**Key Capabilities**:
- **Model Discovery & Deployment**: Explore Azure AI Foundry's model catalog and deploy models to Azure AI Services[1]
- **Knowledge Management**: Create and manage Azure AI Search indexes for RAG systems[1]
- **AI Agent Integration**: Connect with Azure AI Agents and evaluate performance[1]
- **Evaluation Framework**: Run comprehensive text and agent evaluations[1]
- **Prototyping Tools**: GitHub-based prototyping and Azure AI Foundry Labs access[1]

**Status**: Experimental server under active development[1]

## 10. 🏢 Microsoft 365 Agents Toolkit MCP Server

**Purpose**: Essential tools for building AI agents and applications that integrate with Microsoft 365 and Microsoft 365 Copilot[1]

**Key Features**:
- Schema validation for declarative agent manifests[1]
- Sample code retrieval for Microsoft Graph API plugins[1]
- Troubleshooting assistance for common development issues[1]

**Use Cases**:
- "Validate my declarative agent manifest and fix any schema errors"[1]
- "Show me sample code for implementing a Microsoft Graph API plugin"[1]
- "Help me troubleshoot my Teams app authentication issues"[1]

**Recommendation**: Use alongside Microsoft Learn Docs MCP Server for comprehensive M365 development support[1]

## Getting Started

These MCP servers can be set up in **VS Code** (with Agent mode) or **Visual Studio 2022** (version 17.14 or later)[1]. Each server requires specific configuration including connection strings and authentication, but follows a consistent setup pattern across both IDEs[1].

The servers leverage the **Model Context Protocol (MCP)** standard, enabling vendor interoperability and allowing developers to mix and match tools from different vendors in their AI workflow[1].

[1] https://devblogs.microsoft.com/blog/10-microsoft-mcp-servers-to-accelerate-your-development-workflow
