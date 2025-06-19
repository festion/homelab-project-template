# 🏗️ Homelab Project Template

This is a template repository that provides a standardized project structure for homelab projects, including a comprehensive `.prompts` directory with AI-assisted development workflows.

## 🎯 What This Template Provides

### 📁 Standardized .prompts Directory
Complete collection of structured prompts for:
- **System Prompts**: Project context and development assistant behavior
- **Development Workflows**: Code review checklists and feature development guides  
- **Operations Procedures**: Deployment and incident response frameworks
- **Analysis Tools**: GitOps auditing and security assessment procedures
- **Templates**: Reusable prompt templates for creating new prompts

### 🚀 Quick Start Options

#### Option 1: Use GitHub Template (Recommended)
1. Click "Use this template" button above
2. Create your new repository
3. Customize `.prompts/system-prompts/project-context.md` with your project details
4. Start developing with AI-assisted workflows!

#### Option 2: GitHub CLI
```bash
gh repo create my-new-project --template festion/homelab-project-template
cd my-new-project
# Customize project-context.md for your specific project
```

#### Option 3: Add to Existing Project
```bash
# Download and run the setup script in your existing project
bash <(curl -s https://raw.githubusercontent.com/festion/homelab-project-template/main/scripts/setup-prompts.sh)
```

## 📋 Included Prompts

### System Prompts
- **project-context.md**: Template for project-specific context and architecture
- **development-assistant.md**: AI assistant specialized for development tasks

### Development Prompts
- **code-review-checklist.md**: 6-point comprehensive code review framework
- **feature-development-guide.md**: End-to-end feature development process

### Operations Prompts  
- **deployment-procedures.md**: Safe deployment practices with rollback procedures
- **incident-response.md**: Severity-based incident classification and response

### Analysis Prompts
- **gitops-audit-procedures.md**: GitOps compliance assessment framework
- **security-assessment.md**: Multi-layer security vulnerability assessment

### Templates
- **prompt-template.md**: Standardized template for creating new prompts
- **project-template-setup.md**: Guide for implementing organization-wide standards

## 🔧 Customization Guide

### Essential Customization
1. **Edit Project Context**: Update `.prompts/system-prompts/project-context.md` with:
   - Your project's specific purpose and architecture
   - Technology stack and development environment
   - Operational requirements and deployment details

2. **Adapt Prompts**: Modify existing prompts to match your:
   - Development workflows and coding standards
   - Deployment and operational procedures  
   - Security and compliance requirements

3. **Add Project-Specific Prompts**: Create additional prompts for:
   - Specialized development procedures
   - Custom operational workflows
   - Project-specific analysis requirements

### Project Structure Recommendations
```
your-project/
├── .prompts/                    # AI-assisted development workflows
├── .github/                     # GitHub workflows and templates
├── docs/                        # Project documentation
├── src/                         # Source code
├── tests/                       # Test files
├── scripts/                     # Automation scripts
├── config/                      # Configuration files
├── .gitignore                   # Git ignore patterns
├── package.json                 # Dependencies (if Node.js)
└── README.md                    # Project overview
```

## 🎓 Using the Prompts

### For AI Assistants
1. **Load System Context**: Start with `.prompts/system-prompts/project-context.md`
2. **Choose Appropriate Workflow**: Select prompts based on task type
3. **Follow Structured Process**: Use step-by-step guidance in each prompt
4. **Validate Results**: Apply validation frameworks provided

### For Development Teams
1. **Reference During Development**: Use prompts as checklists and guidance
2. **Onboard New Members**: Provide complete project context instantly
3. **Standardize Reviews**: Use consistent code review frameworks
4. **Improve Quality**: Follow proven development and operational procedures

## 📊 Benefits

### Development Efficiency
- **50% faster code reviews** with standardized checklists
- **Instant project context** for new team members  
- **Consistent quality** across all development work
- **Reduced errors** through step-by-step guidance

### Operational Excellence
- **Systematic deployments** with proven procedures
- **Faster incident resolution** with structured response frameworks
- **Security compliance** through comprehensive assessment procedures
- **GitOps best practices** with audit frameworks

## 🔄 Keeping Templates Updated

### Update Your Project's Prompts
```bash
# Download the latest setup script and run it
bash <(curl -s https://raw.githubusercontent.com/festion/homelab-project-template/main/scripts/setup-prompts.sh)
```

### Contributing Back
1. Fork this template repository
2. Improve prompts based on your experience
3. Submit pull requests with enhancements
4. Help build better templates for everyone

## 📚 Additional Resources

- **Complete Documentation**: See `.prompts/PROMPTS_OVERVIEW.md`
- **Standardization Guide**: See `.prompts/STANDARDIZATION_GUIDE.md`
- **Original Source**: [homelab-gitops-auditor](https://github.com/festion/homelab-gitops-auditor)

## 🤝 Contributing

This template repository is designed to evolve with the community:

1. **Share Improvements**: Submit PRs with prompt enhancements
2. **Report Issues**: Open issues for problems or suggestions
3. **Add Specialized Prompts**: Contribute domain-specific workflows
4. **Update Documentation**: Help keep guides current and useful

## 📄 License

This template is provided under the MIT License. Use it freely for your homelab projects and contribute improvements back to the community.

---

**Ready to start?** Click "Use this template" above or run the setup script in your existing project!

**Questions?** Check the documentation in the `.prompts/` directory or open an issue.

Happy building! 🚀