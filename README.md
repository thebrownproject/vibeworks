# 🤖 Claude Code Master Template

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Claude Code](https://img.shields.io/badge/Claude_Code-Compatible-blue.svg)](https://docs.anthropic.com/en/docs/claude-code)
[![BMAD Method](https://img.shields.io/badge/BMAD_Method-Integrated-green.svg)](https://github.com/thebrownproject/BMAD-METHOD)
[![Context7](https://img.shields.io/badge/Context7-Ready-orange.svg)](https://context7.ai)
[![Serena](https://img.shields.io/badge/Serena-Integrated-purple.svg)](https://github.com/thebrownproject/serena)
[![Playwright](https://img.shields.io/badge/Playwright-Ready-red.svg)](https://playwright.dev)
[![Sequential-thinking](https://img.shields.io/badge/Sequential_Thinking-Ready-blue.svg)](https://github.com/modelcontextprotocol/servers)
[![Supabase](https://img.shields.io/badge/Supabase-Ready-green.svg)](https://supabase.com)
[![Brave Search](https://img.shields.io/badge/Brave_Search-Ready-orange.svg)](https://brave.com/search)

> **The ultimate foundation for AI-assisted development projects** - A comprehensive, production-ready template that integrates modern AI development methodologies with battle-tested configurations and workflows.

---

## 📋 Table of Contents

- [🚀 Quick Start](#-quick-start)
- [✨ Features](#-features)
- [🏗️ What's Included](#️-whats-included)
- [📁 Repository Structure](#-repository-structure)
- [🔧 Configuration Options](#-configuration-options)
- [📚 Development Methodologies](#-development-methodologies)
- [🛠️ Advanced Features](#️-advanced-features)
- [📖 Documentation](#-documentation)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)

---

## 🚀 Quick Start

Get up and running with the Claude Code Master Template in 3 simple steps:

### 1. Clone and Setup

```bash
# Clone the master template
git clone git@github.com:thebrownproject/claude-code-master-template.git my-new-project
cd my-new-project

# Remove the original git history and start fresh
rm -rf .git
git init
```

### 2. Choose Your Configuration

```bash
# For Python projects (recommended starting point)
cp claude-configs/claude-python.md CLAUDE.md

# For other languages - adapt the generic CLAUDE.md or create new configs
# See claude-configs/ directory for available options
```

### 3. Initialize Your Project

```bash
# Update BMAD Method to latest version (recommended)
npx bmad-method@latest install

# Initialize your git repository
git add .
git commit -m "Initial commit: Set up from Claude Code Master Template"

# Add your remote and push
git remote add origin YOUR_REPO_URL
git push -u origin main
```

🎉 **You're ready to go!** Your project now includes professional AI development workflows, comprehensive documentation management, and battle-tested configurations.

---

## ✨ Features

### 🎯 **AI-First Development**
- **BMAD Method Integration**: Pre-configured with 10+ specialized AI agents for planning, development, and QA
- **Context7 Documentation**: Intelligent local-first documentation caching and retrieval system
- **Serena Semantic Analysis**: Token-efficient code navigation with hybrid workflow (Serena discovers → Claude Code edits)
- **Playwright Browser Automation**: AI-powered browser testing and web interactions using accessibility tree
- **Sequential-thinking**: Structured problem-solving with dynamic thought processes and revision capabilities
- **Supabase Integration**: Complete database management, branching, and project operations
- **Brave Search**: Comprehensive web search with fresh, unbiased results complementing built-in search

### 🛠️ **Production-Ready Configuration**
- **261+ Configuration Files**: Comprehensive setup covering all aspects of modern development
- **Multi-Language Support**: Extensible language-specific configurations (Python included)
- **Security-First**: Carefully curated permissions and secure development practices

### 📚 **Documentation Excellence**
- **Smart Documentation Management**: 4 specialized Context7 commands for documentation workflows
- **Methodology Integration**: Compatible with leading AI development frameworks
- **Living Documentation**: Templates that evolve with your project

---

## 🏗️ What's Included

| Component | Description | Files | Key Features |
|-----------|-------------|-------|--------------|
| **BMAD Method** | Agile AI-driven development framework | 70+ files | Analyst, PM, Architect, Dev, QA agents |
| **Context7 Integration** | Documentation management system | 5 commands | Local-first, intelligent caching, API integration |
| **Serena Integration** | Token-efficient semantic code analysis | Pre-configured | Hybrid workflow, symbol navigation, memory system |
| **Claude Configurations** | Language-specific development configs | 3+ configs | Python, extensible framework for other languages |
| **MCP Server Setup** | Model Context Protocol integration | 6 servers | Context7, Serena, Playwright, Sequential-thinking, Supabase, Brave Search |
| **Permissions System** | Security and development permissions | Curated settings | File ops, dev tools, web access, package managers |

---

## 📁 Repository Structure

```
claude-code-master-template/
├── 📄 README.md                          # This file
├── 📋 CLAUDE.md                          # Main project instructions
├── 📦 package.json                       # Node.js project configuration (enables Serena)
├── 🔧 .claude/                           # Claude Code configuration
│   ├── settings.local.json               # Permissions and security settings
│   ├── 📚 docs/                          # Documentation cache (Context7 ready)
│   └── ⚡ commands/                       # Custom slash commands
│       ├── BMad/                         # BMAD Method commands
│       │   ├── agents/                   # 10 specialized AI agents
│       │   └── tasks/                    # Development task definitions
│       ├── custom/context7/              # 4 Context7 documentation commands
│       └── imports/                      # Temporary project-specific commands
├── 🧠 .bmad-core/                        # BMAD Method core configuration
│   ├── agents/                           # Core agent definitions (Analyst, PM, etc.)
│   ├── tasks/                            # Task templates and workflows
│   ├── templates/                        # Document templates (PRD, architecture, etc.)
│   ├── workflows/                        # Development workflow definitions
│   └── data/                             # Knowledge base and best practices
├── 🔍 .serena/                           # Serena MCP configuration
│   ├── project.yml                       # Serena project configuration
│   ├── memories/                         # Project knowledge base
│   └── cache/                            # Semantic analysis cache
└── ⚙️ claude-configs/                    # Language-specific configurations
    ├── CLAUDE.md                         # Configuration usage guide
    └── claude-python.md                  # Comprehensive Python dev config
```

---

## 🔧 Configuration Options

### Language-Specific Configurations

The template includes comprehensive configurations for different technology stacks:

#### 🐍 Python Development (`claude-python.md`)
- **Package Management**: UV-based dependency management
- **Testing**: pytest with comprehensive patterns
- **Code Quality**: Ruff formatting and linting
- **Frameworks**: FastAPI, Pydantic v2 patterns
- **Database**: Naming conventions and best practices

#### 🚀 Extensible Framework
Create new language configurations by following the established pattern:

```bash
# Create a new language configuration
cp claude-configs/claude-python.md claude-configs/claude-javascript.md
# Edit to include JavaScript/Node.js specific guidance
```

### MCP Server Configuration

Pre-configured MCP servers include:

- **Context7**: Documentation retrieval and intelligent caching system
- **Serena**: Token-efficient semantic code analysis with hybrid workflow approach
- **Playwright**: AI-powered browser automation using accessibility tree (not screenshots)
- **Sequential-thinking**: Dynamic problem-solving through structured thought processes
- **Supabase**: Complete project management, database operations, and development branching
- **Brave Search**: Comprehensive web search with fresh, unbiased results
- **Extensible**: Easy integration framework for additional MCP servers

#### Hybrid Workflow Benefits
- **Token Efficiency**: Serena's semantic search reduces the need for full file reads
- **User Control**: All code changes go through familiar Claude Code editing interface
- **Smart Discovery**: Use Serena to locate targets, Claude Code to implement changes
- **Knowledge Building**: Persistent memory system for project understanding

---

## 📚 Development Methodologies

### 🎯 BMAD Method (Pre-Installed)

The **Breakthrough Method of Agile AI-Driven Development** comes fully integrated:

#### Planning Phase Agents
- **🔍 Analyst**: Requirements gathering and stakeholder analysis
- **📋 PM**: Project management and coordination
- **🏗️ Architect**: System design and technical architecture

#### Development Phase Agents
- **👥 SM**: Scrum Master for process facilitation
- **💻 Dev**: Development execution and implementation
- **🧪 QA**: Quality assurance and testing

#### Specialized Agents
- **👤 UX Expert**: User experience design and analysis
- **📊 PO**: Product Owner for feature prioritization
- **🤖 BMAD Master**: Overall methodology coordination



---

## 🛠️ Advanced Features

### 📖 Context7 Documentation Management

Four specialized commands for comprehensive documentation workflows:

| Command | Purpose | Use Case |
|---------|---------|----------|
| `/context7:retrieve-docs` | Fresh documentation retrieval | Getting latest library docs |
| `/context7:read-docs` | Local-first reading | Cost-effective doc access |
| `/context7:list-docs` | Cache inventory | Managing documentation cache |
| `/context7:refresh-docs` | Selective updates | Keeping docs current |

### 🔍 Serena Semantic Analysis

Token-efficient code navigation with intelligent semantic tools:

| Tool | Purpose | Use Case |
|------|---------|----------|
| `search_for_pattern` | Find code patterns across codebase | Locating specific functions or patterns |
| `get_symbols_overview` | High-level file structure analysis | Understanding code organization without full reads |
| `find_symbol` | Semantic symbol search | Finding classes, methods, variables |
| `write_memory` | Build project knowledge base | Storing insights for future reference |

#### Hybrid Workflow Advantage
- **Discovery Phase**: Serena locates exact code sections needing changes
- **Edit Phase**: Claude Code's familiar Read → Edit tools for modifications  
- **Review Phase**: User approves all changes through Claude Code interface
- **Efficiency**: Dramatically reduces tokens while maintaining full user control

### 🎭 Playwright Browser Automation

AI-powered browser automation using accessibility tree for reliable, deterministic testing:

| Tool | Purpose | Use Case |
|------|---------|----------|
| `browser_navigate` | Navigate to URLs | Opening web pages for testing |
| `browser_snapshot` | Capture accessibility snapshots | Understanding page structure without vision models |
| `browser_click` | Click elements using accessibility tree | Interacting with buttons, links, forms |
| `browser_type` | Type text into forms | Filling out forms and inputs |
| `browser_evaluate` | Execute JavaScript | Running custom scripts in browser context |

#### Key Advantages
- **No Screenshots Required**: Uses structured accessibility data instead of vision models
- **Fast & Deterministic**: Reliable automation without pixel-based ambiguity
- **Multi-Browser Support**: Chrome, Firefox, WebKit compatibility
- **Real Browser Environment**: Full JavaScript execution and modern web features

### 🧠 Sequential-thinking Problem Solving

Dynamic and reflective problem-solving through structured thought processes:

| Feature | Purpose | Use Case |
|---------|---------|----------|
| Dynamic Thought Sequences | Adjustable reasoning steps | Complex planning and analysis |
| Revision Capabilities | Question and revise previous thoughts | Iterative problem refinement |
| Branching Approaches | Explore alternative solutions | Decision tree exploration |
| Session State Management | Maintain context across interactions | Long-running problem solving |

#### Problem-Solving Benefits
- **Adaptive Planning**: Adjust reasoning depth based on problem complexity
- **Iterative Refinement**: Revise and improve solutions through structured thinking
- **Transparent Process**: Clear visibility into AI reasoning steps
- **Complex Analysis**: Handle multi-faceted problems systematically

### 🗄️ Supabase Database Management

Complete Supabase project management with development-safe workflows:

| Tool Category | Purpose | Key Tools |
|---------------|---------|-----------|
| **Project Management** | List, create, manage projects | `list_projects`, `create_project`, `get_project` |
| **Database Operations** | SQL execution and schema management | `execute_sql`, `apply_migration`, `list_tables` |
| **Development Branching** | Safe testing environments | `create_branch`, `merge_branch`, `reset_branch` |
| **Debugging & Monitoring** | Logs and project insights | `get_logs`, `get_advisors` |

#### Development Workflow Benefits
- **Safe Testing**: Development branches for risk-free experimentation
- **Read-Only Mode**: Connect to production data safely
- **Comprehensive Management**: 20+ tools for complete project control
- **Migration Support**: Systematic database evolution tracking

### 🔍 Brave Search Web Research

Comprehensive web search capabilities that complement Claude's built-in search:

| Feature | Purpose | Use Case |
|---------|---------|----------|
| Fresh Results | Get the most current information | Breaking news, recent developments, latest documentation |
| Unbiased Search | Independent search without filter bubbles | Research, fact-checking, diverse perspectives |
| Comprehensive Coverage | Wide range of sources and content types | Market research, technical resources, academic content |
| API Integration | Structured search results for AI processing | Data gathering, content analysis, research automation |

#### Complementary Search Strategy
- **Built-in Search**: Quick, conversational queries and general knowledge
- **Brave Search**: Fresh results, comprehensive research, current events, and specialized content
- **Combined Power**: Best of both worlds for thorough information gathering

### 🔐 Security-First Permissions

Carefully curated permissions system:

- ✅ **Development Operations**: File management, git operations, testing
- ✅ **Package Management**: npm, pip, cargo, etc.
- ✅ **Documentation Access**: Trusted sources (Anthropic, GitHub, MDN)
- ❌ **Restricted Operations**: Potentially dangerous system commands

### 🚀 GitHub CLI Integration

Ready for seamless GitHub operations:

- Repository management
- Pull request workflows
- Issue tracking
- Actions integration

---

## 📖 Documentation

### 📚 Included Guides

- **[CLAUDE.md](CLAUDE.md)**: Complete template overview and usage instructions
- **[claude-configs/](claude-configs/)**: Language-specific configuration guides
- **[.bmad-core/](/.bmad-core/)**: BMAD Method documentation and workflows

### 🌐 External Resources

- **[Claude Code Documentation](https://docs.anthropic.com/en/docs/claude-code)**: Official Claude Code guide
- **[BMAD Method](https://github.com/thebrownproject/BMAD-METHOD)**: Complete BMAD methodology

### 🔄 Staying Updated

```bash
# Update BMAD Method to latest version
npx bmad-method@latest install

# The template is designed to evolve - watch this repository for updates
```

---

## 🤝 Contributing

We welcome contributions to improve the Claude Code Master Template!

### 🎯 Areas for Contribution

- **New Language Configurations**: Add support for additional programming languages
- **Enhanced MCP Integrations**: Develop new MCP server configurations
- **Improved Workflows**: Enhance BMAD Method tasks and templates
- **Documentation**: Improve guides and examples

### 📝 How to Contribute

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### 🐛 Reporting Issues

Found a bug or have a suggestion? [Open an issue](https://github.com/thebrownproject/claude-code-master-template/issues) with:

- Clear description of the problem or suggestion
- Steps to reproduce (for bugs)
- Your environment details
- Expected vs actual behavior

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- **[Anthropic](https://anthropic.com)** for Claude Code and Claude AI
- **[Cole Medin](https://github.com/coleam00)** for development patterns and Python configuration inspiration
- **[BMAD Method](https://github.com/thebrownproject/BMAD-METHOD)** for agile AI-driven development framework
- **[Context7](https://context7.ai)** for intelligent documentation management
- **[Serena](https://github.com/thebrownproject/serena)** for token-efficient semantic code analysis
- **[Microsoft Playwright](https://playwright.dev)** for browser automation and testing capabilities
- **[Model Context Protocol](https://modelcontextprotocol.io)** for sequential-thinking problem-solving framework
- **[Supabase](https://supabase.com)** for comprehensive database management and development workflows
- **[Brave Search](https://brave.com/search)** for providing fresh, unbiased web search capabilities

---

<div align="center">

**Ready to revolutionize your development workflow?**

⭐ Star this repository • 🍴 Fork it • 📢 Share it

[Get Started](#-quick-start) • [View Documentation](CLAUDE.md) • [Report Issues](https://github.com/thebrownproject/claude-code-master-template/issues)

</div># vibeworks
