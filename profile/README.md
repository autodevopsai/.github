# AutoDevOps.ai

**Your code commits. Our agents handle the rest.**

AI micro-agents that eliminate 80% of DevOps busywork. Zero platform migration required.

## 🚀 Quick Start

```bash
# TypeScript/Node.js
npm install -D @autodevopsai/verifier

# Python  
pip install autodevopsai-verifier

# Go
go get github.com/autodevopsai/verifier-go
```

## 📦 Available Packages

| Language | Repository | Package Registry | Status |
|----------|------------|-----------------|---------|
| TypeScript/Node | [verifier-ts](https://github.com/autodevopsai/verifier-ts) | [@autodevopsai/verifier](https://npmjs.com/package/@autodevopsai/verifier) | 🚧 Coming Soon |
| Python | [verifier-py](https://github.com/autodevopsai/verifier-py) | [autodevopsai-verifier](https://pypi.org/project/autodevopsai-verifier) | 🚧 Coming Soon |
| Go | [verifier-go](https://github.com/autodevopsai/verifier-go) | pkg.go.dev | 🚧 Coming Soon |
| Kotlin/JVM | [verifier-kotlin](https://github.com/autodevopsai/verifier-kotlin) | Maven Central | 🚧 Coming Soon |

## 🚨 The Problem

Every PR wastes 45+ minutes on:
- 🎨 Style nitpicks across multiple languages
- 🔒 Security reviews and vulnerability scanning
- 📚 Documentation updates that never happen
- ✍️ Writing tests for edge cases
- 🔍 Code review back-and-forth

That's **112.5 hours per developer per year**. Just on repetitive tasks.

## ✨ The Solution

AutoDevOps inserts lightweight, LLM-powered micro-agents into your existing Git hooks and CI/CD pipeline. No new platforms. No migrations. Just intelligent automation that runs exactly where your work already happens.

### How It Works

1. **Install** the package for your language
2. **Configure** agents in `.shadow/hooks.yaml`
3. **Commit** code as usual
4. **Review** AI suggestions before applying

```yaml
# .shadow/hooks.yaml
hooks:
  pre_commit:
    agents:
      - id: CQ-003  # Polyglot Linter
        auto_fix: true
      - id: SC-001  # Security Scanner
        blocking: true
  
  post_merge:
    agents:
      - id: DD-001  # ADR Writer
        template: standard
```

## 🤖 Agent Catalog

| Agent | Purpose | Hook | Auto-fix |
|-------|---------|------|----------|
| **CQ-003** Polyglot Linter | Multi-language linting | `pre_commit` | ✅ |
| **SC-001** Security Scanner | Find vulnerabilities | `pre_commit` | ❌ |
| **DD-010** Intent Generator | Turn tickets into specs | `issue_created` | N/A |
| **DD-001** ADR Writer | Document decisions | `post_merge` | N/A |
| **CQ-001** Test Generator | Create test scaffolding | `pre_commit` | ✅ |

[View complete agent list →](https://www.autodevops.ai/directory)

## 📊 Expected Impact

Based on early implementations:
- **30% faster** PR cycle time
- **50% fewer** production bugs
- **100%** documentation coverage
- **40% reduction** in dev hours on repetitive tasks

## 🏗️ Architecture

```
Git Hook → Orchestrator → Agent Selection → LLM Processing → Review → Apply
```

Agents run in parallel when possible, respect your existing workflow, and never make changes without review (unless explicitly configured).

## 🤝 Contributing

We welcome contributions! Each package repository accepts PRs for:
- New agent implementations
- Language-specific improvements
- Bug fixes and performance enhancements

See [CONTRIBUTING.md](https://github.com/autodevopsai/.github/blob/main/CONTRIBUTING.md) for guidelines.

## 📖 Resources

- [Documentation Wiki](https://github.com/autodevopsai/.github/wiki)
- [Agent Development Guide](https://github.com/autodevopsai/.github/wiki/Agent-Development)
- [Integration Examples](https://github.com/autodevopsai/.github/wiki/Integrations)

## 🏢 About

AutoDevOps.ai is building the future of automated development operations. We believe developers should focus on solving problems, not repetitive tasks.

## 📄 License

MIT - See individual package repositories for details.

---

<p align="center">
  <a href="https://autodevops.ai">Website</a> •
  <a href="https://twitter.com/autodevopsai">Twitter</a> •
  <a href="mailto:hello@mail.autodevops.ai">Contact</a>
</p>
