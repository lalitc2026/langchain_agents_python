# LangChain Agents with MCP Integration

A comprehensive tutorial series demonstrating advanced LangChain agent patterns with Model Context Protocol (MCP) integration.

## Overview

This project provides hands-on examples of building sophisticated AI agents using LangChain, focusing on MCP server integration, agent state management, and multi-agent architectures. The tutorials cover both local and external MCP server connections, context handling, and advanced agent patterns.

## Features

- **MCP Server Integration**: Connect LangChain agents with MCP servers for extended tool capabilities
- **Agent State Management**: Implement persistent state and context across agent interactions
- **Multi-Agent Systems**: Build hierarchical agent architectures with specialized sub-agents
- **Real-world Tools**: Integration with web search, file access, and external APIs
- **Memory and Checkpoints**: Persistent conversation state using LangGraph checkpointers

## Project Structure

```
├── requirements.txt                 # Python dependencies
├── mcp_and_agent_state/            # Tutorial notebooks
│   ├── 1_mcp1.ipynb               # Local MCP server setup
│   ├── 2_mcp2.ipynb               # External MCP server integration
│   ├── 3_agent_state.ipynb        # Agent context and state
│   ├── 4_runtime_context.ipynb    # Runtime state management
│   ├── 5_multi_agent.ipynb        # Multi-agent architectures
│   └── resources/
│       └── mcp_server.py         # Sample MCP server implementation
└── README.md                      # This file
```

## Prerequisites

- Python 3.8+
- Virtual environment (recommended)
- API keys for various services (OpenAI, Anthropic, Tavily, etc.)

## Installation

1. Clone or download this repository
2. Create a virtual environment:
   ```bash
   python -m venv .venv
   ```
3. Activate the virtual environment:
   - Windows: `.venv\Scripts\activate`
   - macOS/Linux: `source .venv/bin/activate`
4. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Environment Setup

Create a `.env` file in the root directory with your API keys:

```env
OPENAI_API_KEY=your_openai_key
ANTHROPIC_API_KEY=your_anthropic_key
TAVILY_API_KEY=your_tavily_key
# Add other required API keys as needed
```

## Tutorials

### 1. Local MCP Server (`1_mcp1.ipynb`)
- Setting up a local MCP server using FastMCP
- Creating custom tools (web search, file access)
- Connecting LangChain agents to MCP servers
- Handling Windows-specific asyncio issues in Jupyter

### 2. External MCP Server (`2_mcp2.ipynb`)
- Connecting to external MCP servers (travel booking API)
- Using streamable HTTP transport
- Agent memory with checkpointers
- Real-world API integration

### 3. Agent State (`3_agent_state.ipynb`)
- Implementing context schemas
- Runtime context in tools
- Dynamic state management
- User preference handling

### 4. Runtime Context (`4_runtime_context.ipynb`)
- Reading and writing to agent state
- Persistent state across conversations
- State-based tool behavior
- Memory management

### 5. Multi-Agent Systems (`5_multi_agent.ipynb`)
- Creating specialized sub-agents
- Hierarchical agent architectures
- Inter-agent communication
- Complex task delegation

## Key Technologies

- **LangChain**: Core agent framework
- **LangGraph**: Graph-based agent orchestration
- **MCP (Model Context Protocol)**: Standardized tool interface
- **FastMCP**: Python MCP server framework
- **Tavily**: Web search integration
- **LangSmith**: Agent monitoring and debugging

## Sample MCP Server

The `resources/mcp_server.py` provides a sample MCP server with:
- Web search tool using Tavily
- GitHub file access for LangChain documentation
- Custom prompts for LangChain-related queries

## Usage

1. Start Jupyter Lab:
   ```bash
   jupyter lab
   ```
2. Open the notebooks in order `1_mcp1.ipynb` through `5_multi_agent.ipynb`
3. Run cells sequentially to understand each concept
4. Modify examples to experiment with different configurations

## Contributing

This is an educational project. Feel free to:
- Report issues with the tutorials
- Suggest improvements to examples
- Add new tutorial notebooks
- Update dependencies

## License

This project is for educational purposes. Check individual package licenses for production use.

## Resources

- [LangChain Documentation](https://python.langchain.com/)
- [MCP Specification](https://modelcontextprotocol.io/)
- [LangGraph Guide](https://langchain-ai.github.io/langgraph/)
- [FastMCP](https://github.com/jlowin/fastmcp)# langchain_agents_python
