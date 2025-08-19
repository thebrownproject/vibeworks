# Claude Configurations

This folder contains language-specific Claude Code configuration files that provide comprehensive guidance for different technology stacks.

## Available Configurations

### claude-python.md
Comprehensive Python development configuration including:
- UV package management
- Testing with pytest
- Code formatting with Ruff
- Pydantic v2 patterns
- Database naming conventions
- FastAPI development patterns

## How to Use

When starting a new project:

1. **Copy the master template** to your new project location
2. **Choose your configuration**: Look at the available configs in this folder
3. **Replace CLAUDE.md**: Copy your chosen config to replace the generic `CLAUDE.md` in the project root
4. **Customize**: Adapt the configuration for your specific project needs

### Example Workflow

```bash
# Copy master template
cp -r master-template my-new-python-project
cd my-new-python-project

# Replace generic CLAUDE.md with Python-specific config
cp claude-configs/claude-python.md CLAUDE.md

# Customize for your project
# Edit CLAUDE.md to add project-specific rules, dependencies, etc.
```

## Adding New Configurations

To add support for new languages or frameworks:

1. Create a new file: `claude-{language}.md`
2. Include comprehensive guidance for that technology stack
3. Follow the pattern established in `claude-python.md`
4. Update this README to document the new configuration

## Configuration Structure

Each configuration should include:

- **Development Philosophy** (KISS, YAGNI, design principles)
- **Code Structure & Modularity** (file limits, architecture patterns)
- **Development Environment** (package managers, tooling)
- **Style & Conventions** (formatting, naming, docstrings)
- **Testing Strategy** (TDD, testing patterns, organization)
- **Error Handling** (exceptions, logging)
- **Performance Considerations**
- **Security Best Practices**
- **Documentation Standards**

This ensures consistent, high-quality guidance across all technology stacks.