# Homelab Project Template

A comprehensive template for homelab projects with integrated MCP (Model Context Protocol) server support, GitHub Actions, and standardized project structure.

## Features

- 🏗️ **Standardized Project Structure** - Pre-configured directories for API, dashboard, scripts, and documentation
- 🤖 **MCP Server Integration** - Built-in support for Claude AI assistant with pre-configured MCP servers
- 🔄 **GitHub Actions** - Ready-to-use CI/CD workflows for testing, building, and deployment
- 📚 **Documentation Templates** - Complete documentation structure with setup guides and troubleshooting
- 🛠️ **Development Scripts** - Automated setup, validation, and update scripts
- 🎯 **Multiple Project Types** - Support for API-only, dashboard-only, or full-stack projects

## Quick Start

1. **Use this template** by clicking "Use this template" on GitHub or clone directly:
   ```bash
   git clone https://github.com/festion/homelab-project-template.git my-project
   cd my-project
   ```

2. **Initialize your project**:
   ```bash
   ./scripts/setup.sh
   ```

3. **Configure your project** by editing `template-config.json`:
   ```json
   {
     "project": {
       "name": "my-awesome-project",
       "description": "Description of your project",
       "type": "fullstack"
     }
   }
   ```

4. **Start developing** - The template provides:
   - API development in `/api`
   - Dashboard development in `/dashboard`
   - Utility scripts in `/scripts`
   - Documentation in `/docs`

## Project Types

- **generic** - Basic project structure
- **api** - Backend API project with Express.js template
- **dashboard** - Frontend dashboard with React template
- **fullstack** - Complete full-stack application
- **automation** - Script-based automation project

## MCP Server Support

This template includes pre-configured MCP servers for enhanced AI assistance:

- **Filesystem** - File operations and directory management
- **GitHub** - Repository management and GitHub API integration
- **Home Assistant** - Home automation system integration
- **Network FS** - Network file system operations
- **Directory Polling** - File system monitoring

See [docs/MCP_CONFIGURATION.md](docs/MCP_CONFIGURATION.md) for detailed configuration.

## Documentation

- [Setup Guide](docs/SETUP.md) - Detailed setup instructions
- [Customization Guide](docs/CUSTOMIZATION.md) - How to customize the template
- [MCP Configuration](docs/MCP_CONFIGURATION.md) - MCP server setup and usage
- [Troubleshooting](docs/TROUBLESHOOTING.md) - Common issues and solutions

## Examples

Check the `/examples` directory for:
- Basic project setup
- Advanced customization examples
- Integration patterns

## Scripts

- `scripts/setup.sh` - Initialize new project from template
- `scripts/validate-config.sh` - Validate project configuration
- `scripts/update-template.sh` - Update template to latest version

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

## License

MIT License - see [LICENSE](LICENSE) for details.

## Support

- 📖 Check the [documentation](docs/)
- 🐛 Report issues on [GitHub Issues](https://github.com/festion/homelab-project-template/issues)
- 💬 Join discussions in [GitHub Discussions](https://github.com/festion/homelab-project-template/discussions)