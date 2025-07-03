# Cursor Rules: RIPER CAT Methodology & Development Standards

This repository contains a comprehensive set of **Cursor IDE rules** that implement the **RIPER CAT methodology** - an AI-assisted development protocol designed for enterprise-grade software development.

## 🚀 What is RIPER CAT?

**RIPER CAT** is a structured operational protocol for AI-assisted development that provides:

- **8 Distinct Development Modes** with clear boundaries and responsibilities
- **Strict Mode Transitions** preventing unauthorized AI assumptions or code rewrites
- **Enterprise-Grade Standards** for database, frontend, and backend development
- **Comprehensive Documentation Ecosystem** with cross-referenced specialized rules

### The 8 Modes

1. **RESEARCH** - Passive observation and deep analysis
2. **INNOVATE** - Brainstorming and exploration
3. **PLAN** - Exhaustive implementation specifications
4. **EXECUTE** - Strict implementation following approved plans
5. **REVIEW** - Validation against specifications
6. **COMMIT** - Documentation updates and git operations
7. **AI REVIEW** - Peer review analysis
8. **TROUBLESHOOT** - Root cause analysis

## 📁 Repository Structure

```
rules/
├── riper.mdc                          # Core RIPER CAT operational protocol
├── page-layout-standards.mdc         # Frontend layout consistency standards
├── supabase-*.mdc                    # Database and backend development standards
├── cursor_rules.mdc                  # Meta-rules for maintaining cursor rules
├── rules-index.mdc                   # Master index of all rules
└── mcp-supabase-integration.mdc      # Model Context Protocol tools
```

## 🎯 Quick Start

### 1. Install Cursor IDE
Download [Cursor IDE](https://cursor.sh/) (fork of VS Code with AI integration)

### 2. Add Rules to Your Project
```bash
# In your project root
mkdir -p .cursor/rules
cd .cursor/rules

# Download the rules you need
curl -O https://raw.githubusercontent.com/HuntsDesk/cursor_rules/main/rules/riper.mdc
curl -O https://raw.githubusercontent.com/HuntsDesk/cursor_rules/main/rules/page-layout-standards.mdc
# Add other rules as needed
```

### 3. Start Using RIPER CAT
In your Cursor IDE chat, always begin with mode declaration:
```
[MODE: RESEARCH]
I need to understand how authentication works in this codebase.
```

## 🏗️ Architecture Support

These rules are designed for modern web development stacks:

- **Frontend**: React 18+, Vite 6+, TypeScript
- **Backend**: Supabase Edge Functions (Deno)
- **Database**: PostgreSQL with Row Level Security
- **Styling**: Tailwind CSS with responsive design patterns
- **State Management**: React Query v5+

## 📖 Rule Categories

### Core Operational Protocol
- **[riper.mdc](rules/riper.mdc)** - Complete RIPER CAT methodology

### Frontend Development
- **[page-layout-standards.mdc](rules/page-layout-standards.mdc)** - React component layouts, responsive design, mobile patterns

### Backend & Database
- **[supabase-edge-functions.mdc](rules/supabase-edge-functions.mdc)** - Edge function development standards
- **[supabase-rls-policies.mdc](rules/supabase-rls-policies.mdc)** - Database security policies
- **[supabase-create-migration.mdc](rules/supabase-create-migration.mdc)** - Database migration best practices
- **[mcp-supabase-integration.mdc](rules/mcp-supabase-integration.mdc)** - Direct database operations

### Development Infrastructure
- **[cursor_rules.mdc](rules/cursor_rules.mdc)** - Guidelines for creating and maintaining rules
- **[rules-index.mdc](rules/rules-index.mdc)** - Master index for AI agent navigation

## 🎨 Key Features

### Intelligent Mode Management
```typescript
// RIPER CAT enforces strict boundaries
[MODE: PLAN]
1. Update UserProfile component
2. Add responsive mobile layout
3. Implement dark mode toggle

[MODE: EXECUTE]
// Only implements what was planned - no creative interpretation
```

### Enterprise Layout System
```tsx
// Consistent, responsive layouts
<PageContainer 
  disablePadding={false} 
  className="pt-6 pb-6 md:pb-12 mx-auto px-4" 
  maxWidth="6xl"
>
  {children}
</PageContainer>
```

### Database Security First
```sql
-- RLS policies are required for all tables
CREATE POLICY "users_own_data" ON profiles
FOR ALL USING (auth.uid() = user_id);
```

## 📚 Usage Examples

### Basic Development Workflow
```bash
# 1. Start with research
[MODE: RESEARCH]
Analyze the current authentication system

# 2. Plan changes
[MODE: PLAN] 
Create implementation spec for 2FA

# 3. Execute plan
[MODE: EXECUTE]
Implement exactly what was planned

# 4. Review results
[MODE: REVIEW]
Validate against plan requirements
```

### Specialized Rule Integration
```bash
# Reference multiple specialized rules
[MODE: PLAN]
- Use page-layout-standards.mdc for UI components
- Apply supabase-rls-policies.mdc for data security
- Follow supabase-edge-functions.mdc for API endpoints
```

## 🔧 Integration with Popular Tools

### GitHub Actions
```yaml
# Sync rules automatically
- name: Update Cursor Rules
  run: |
    curl -O https://raw.githubusercontent.com/HuntsDesk/cursor_rules/main/rules/riper.mdc
```

### VS Code / Cursor
Add to your `.vscode/settings.json`:
```json
{
  "cursor.rules": [
    ".cursor/rules/riper.mdc",
    ".cursor/rules/page-layout-standards.mdc"
  ]
}
```

## 🌟 Community Contributions

### Community Adaptations

- **[RIPER-5 Mode](https://forum.cursor.com/t/i-created-an-amazing-mode-called-riper-5-mode-fixes-claude-3-7-drastically/65516)** by robotlovehuman - A streamlined 5-mode adaptation focusing on Research, Innovate, Plan, Execute, Review for fixing Claude 3.7 behavior in complex workflows

The RIPER methodology continues to evolve through community contributions and real-world testing across different development environments.

## 🤝 Contributing

We welcome contributions! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

### Rule Development Process
1. Follow the [cursor_rules.mdc](rules/cursor_rules.mdc) meta-standards
2. Cross-reference with [rules-index.mdc](rules/rules-index.mdc)
3. Test rules with real-world development scenarios
4. Update documentation and examples

## 📈 Benefits

- **🚀 Faster Development** - Structured approach eliminates context switching
- **🎯 Higher Quality** - Strict validation prevents implementation drift
- **📖 Better Documentation** - Integrated documentation standards
- **🔒 Enhanced Security** - Security-first database and API patterns
- **📱 Mobile-First Design** - Responsive layout standards built-in
- **🔄 Consistent Results** - Reproducible development patterns

## 🏢 Enterprise Features

- **Audit Trails** - Every mode transition is tracked
- **Security Standards** - Built-in RLS, authentication, and API security
- **Performance Optimization** - Layout and query optimization patterns
- **Scalability Patterns** - Database and frontend scaling best practices
- **Documentation Integration** - Self-updating documentation systems

## 📄 License

MIT License - see [LICENSE](LICENSE) for details.

## 🙏 Acknowledgments

Built for modern AI-assisted development with [Cursor IDE](https://cursor.sh/). Inspired by enterprise development practices and the need for structured AI collaboration.

---

**Ready to transform your development workflow?** Start with `riper.mdc` and experience the power of structured AI-assisted development.
