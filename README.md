# AICommit
[简体中文](README-zh_cn.md)

[![Version](https://img.shields.io/jetbrains/plugin/v/21289-aicommit.svg)](https://plugins.jetbrains.com/plugin/21289-aicommit)
[![Downloads](https://img.shields.io/jetbrains/plugin/d/21289-aicommit.svg)](https://plugins.jetbrains.com/plugin/21289-aicommit)


[![AI Commit](./assets/social_preview.jpg)](https://youtu.be/sDG8cx6i_kM "AI Commit")

Still the best AI commit messages for JetBrains IDEs.

Save 30+ minutes daily writing commit messages. Generate precise, context-aware messages in one click. Privacy-first with local processing. Trusted by 19,000+ developers worldwide.

## Quick Links

- [Install Plugin for Free](https://plugins.jetbrains.com/plugin/21289-aicommit/)
- [FAQ](./FAQ.md)
- [Bug Report](https://github.com/AICommitApp/community/issues)
- [EULA](./EULA.md)

## Why AICommit

- **One-Click Generation**: Generate commit messages instantly from the JetBrains VCS commit panel.
- **Prompt Lab & Provider Switch**: Pick provider/model, apply prompt templates, and review generation history in one place.
- **Custom Templates**: Use built-in templates or create your own for Conventional Commits, release notes, and bugfix workflows.
- **Multi-Provider AI**: OpenAI, Azure OpenAI, Google Gemini, Anthropic Claude, and Ollama (local models).
- **Privacy-First Local Mode**: Use Ollama for local processing when your workflow requires stronger privacy control.

## Latest Updates (v3.4.4 - 2026-02-26)

- Added catalog-based model management for more consistent provider/model selection.
- OpenAI now defaults to the `responses` endpoint mode.
- Improved stability for streaming responses and model list refresh.
- Preserved prompt drafts when switching providers or models.
- Improved error handling, localization, and setup guidance when API token is missing.

## Installation

- Using IDE built-in plugin system:

  <kbd>Settings/Preferences</kbd> > <kbd>Plugins</kbd> > <kbd>Marketplace</kbd> > <kbd>Search for "AICommit"</kbd> >
  <kbd>Install Plugin</kbd>

## Configuring Provider API Key
In AICommit settings, choose your provider (OpenAI / Azure OpenAI / Gemini / Claude / Ollama) and configure the required API key or endpoint. Use "Verify" to confirm your configuration before generation.

## Getting Started
1. Install the plugin and open AICommit in your JetBrains IDE.
2. Select provider and model, then verify your API key/endpoint settings.
3. Adjust Prompt Lab (template, custom prompt, default template, recent commit context).
4. Click **Generate**, then insert the result into the Commit panel.

### One-Click Generation

![commit_action](assets/action.png)

### Prompt Lab & Provider Switch

![tool_window](assets/toolwindow.png)

### Custom Templates

![prompt_lab](assets/prompt_lab.png)

---

## Credit
- [AICommit](https://github.com/Nutlope/aicommits):A CLI that writes your git commit messages for you with AI. Never write a commit message again.
- [Openai-Kotlin](https://github.com/aallam/openai-kotlin): Kotlin client for OpenAI's API with multiplatform and coroutines capabilities.
- [java-diff-utils](https://github.com/java-diff-utils/java-diff-utils)
- [knuddelsgmbh/jtokkit](https://github.com/knuddelsgmbh/jtokkit)
- Plugin based on the [IntelliJ Platform Plugin Template][template].
- Deja Vu by Cykarl https://soundcloud.com/cykarl
  Creative Commons — Attribution 3.0 Unported — CC BY 3.0
  Free Download / Stream: https://bit.ly/3IPXpnU
  Music promoted by Audio Library https://youtu.be/-tPlIz3eov4

[template]: https://github.com/JetBrains/intellij-platform-plugin-template
