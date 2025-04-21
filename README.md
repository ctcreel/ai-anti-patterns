# AI Anti-Patterns

**A shared guide to help developers avoid common coding anti-patterns when working with AI pair programming tools.**

AI-assisted development is here to stay. Tools like Claude, Cursor, and ChatGPT are powerful, but they often reproduce the same mistakes developers have been making for decades — because that’s what they’ve been trained on.

This project helps you break that cycle.

`ai-anti-patterns` provides a structured, extensible foundation for guiding AI tools toward writing clean, maintainable, and idiomatic code — by avoiding the most common anti-patterns seen in real-world projects.

---

## Purpose

This repository aims to:

- Document common anti-patterns AI models tend to reproduce
- Provide actionable guidance to avoid them
- Offer tool-specific configuration templates and examples
- Help individuals and teams establish consistent standards when working with AI

---

## Supported Tools

Each AI model has its own folder, including setup files and guidance:

| Tool      | File/Folders | Purpose                                                                 |
|-----------|--------------|-------------------------------------------------------------------------|
| Claude    | `GENERAL.md` | Shared behavior and anti-pattern guidance for Claude Code              |
| Cursor    | `CURSOR.md`  | Explanation of `.cursor/rules.toml` configuration                      |
| ChatGPT   | `GENERAL.md` | Use `GENERAL.md` as the prompt basis for ChatGPT (see notes below)      |

> 💡 **Note:** The `GENERAL.md` file is designed to be tool-agnostic and can be used as the base prompt for ChatGPT sessions or any other AI assistant that benefits from structured behavioral guidance.

## Getting Started

To use this project:

1. Copy the relevant configuration files into your project
2. Customize them based on your team’s architecture and style
3. Share with your team or embed in your development environment
4. Adapt the anti-pattern guidance to your language or tooling stack
5. Submit a pull request to help others benefit from what you’ve improved

---

## Contributing

We welcome PRs that:

- Expand the anti-pattern list or improve existing examples
- Add language-specific code examples (e.g., Go, Ruby, Rust)
- Include new model/tool support (e.g., Copilot, Cody, StarCoder)
- Improve prompt engineering or prompt organization
- Help AI tools produce better results across different workflows

See [`CONTRIBUTING.md`](CONTRIBUTING.md) for contribution guidelines.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## Acknowledgments

This project was started to help the developer community write better code *with* AI — not despite it. Thanks to everyone working to make AI pair programming simpler, more effective, and more human-aware.
