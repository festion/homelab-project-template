# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **homelab project template** repository that generates structured projects with integrated AI assistant support through MCP (Model Context Protocol) servers. It's a scaffolding tool that creates complete project structures with standardized tooling, not a specific application.

## Key Commands

### Project Initialization
```bash
# Initialize a new project from template
./scripts/setup.sh

# Validate project configuration
./scripts/validate-config.sh

# Update template to latest version  
./scripts/update-template.sh
```

### API Development (Express.js)
```bash
cd api/
npm install                    # Install dependencies
npm run dev                    # Start development server with nodemon
npm run start                  # Start production server
npm test                       # Run Jest tests
npm run test:watch             # Run tests in watch mode
npm run test:coverage          # Run tests with coverage
npm run lint                   # Run ESLint
npm run lint:fix              # Fix ESLint issues
npm run format                # Format code with Prettier
```

### Dashboard Development (React + Vite)
```bash
cd dashboard/
npm install                    # Install dependencies  
npm run dev                    # Start Vite development server
npm run build                  # Build for production
npm run preview               # Preview production build
npm test                      # Run Jest tests
npm run test:watch            # Run tests in watch mode
npm run test:coverage         # Run tests with coverage
npm run lint                  # Run ESLint
npm run lint:fix             # Fix ESLint issues
npm run format               # Format code with Prettier
```

## Architecture

### Template Structure
- **`template-config.json`** - Central configuration defining project type, features, and MCP servers
- **`scripts/setup.sh`** - Main initialization script (482 lines) that generates projects
- **`api/`** - Express.js API template with security, logging, authentication
- **`dashboard/`** - React dashboard template with Material-UI, Redux, routing
- **`docs/`** - Documentation templates and guides
- **`.github/workflows/`** - GitHub Actions CI/CD templates

### Technology Stack
- **Backend**: Express.js 4.18.2, Winston logging, JWT auth, bcryptjs, rate limiting
- **Frontend**: React 18.2.0, Vite 4.4.5, Material-UI 5.14.5, Redux Toolkit, Recharts
- **Testing**: Jest for both frontend/backend, React Testing Library, Supertest
- **Linting**: ESLint (Standard config for backend, React config for frontend)
- **CI/CD**: GitHub Actions with Node.js 16,18,20 matrix testing

### Project Types Supported
- **`generic`** - Basic project structure
- **`api`** - Backend API with Express.js
- **`dashboard`** - Frontend dashboard with React  
- **`fullstack`** - Complete full-stack application
- **`automation`** - Script-based automation project

## MCP Server Integration

The template's standout feature is comprehensive AI assistant integration through MCP servers:

### Available MCP Servers
1. **Filesystem** - File operations and directory management
2. **GitHub** - Repository management and GitHub API integration
3. **Home Assistant** - Home automation system integration
4. **Network FS** - Network file system operations
5. **Directory Polling** - File system monitoring
6. **Proxmox** - Virtualization platform integration
7. **TrueNAS** - Storage system management  
8. **WikiJS** - Documentation system integration

### Configuration Location
- Main config: `template-config.json` (lines 11-59)
- Generated MCP config: `.mcp.json` (created by setup script)

## Development Workflow

1. **Configure** - Edit `template-config.json` to specify project type and features
2. **Initialize** - Run `./scripts/setup.sh` to generate project structure
3. **Install** - Run `npm install` in generated `api/` and/or `dashboard/` directories
4. **Develop** - Use respective npm scripts for development, testing, linting
5. **CI/CD** - GitHub Actions automatically test on Node.js 16,18,20

## Key Files

### Configuration
- **`template-config.json`** - Main template configuration
- **`api/package.json`** - Express.js dependencies and scripts  
- **`dashboard/package.json`** - React dependencies and scripts

### Core Scripts
- **`scripts/setup.sh`** - Primary project generation script
- **`scripts/validate-config.sh`** - Configuration validation
- **`scripts/update-template.sh`** - Template updates

### Generated Entry Points
- **`api/src/server.js`** - Express.js server entry point (generated)
- **`dashboard/src/App.jsx`** - React app entry point (generated)

## Testing

- **API**: Jest with Supertest for HTTP testing
- **Dashboard**: Jest with React Testing Library and jsdom
- **Coverage**: Configured for both projects with HTML reports
- **CI**: Automated testing on multiple Node.js versions via GitHub Actions

The template generates production-ready projects with comprehensive tooling, security best practices, and cutting-edge AI assistant integration through MCP servers.