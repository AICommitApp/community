# AICommit
[中文简体](README-zh_cn.md)

[![Version](https://img.shields.io/jetbrains/plugin/v/21289-aicommit.svg)](https://plugins.jetbrains.com/plugin/21289-aicommit)
[![Downloads](https://img.shields.io/jetbrains/plugin/d/21289-aicommit.svg)](https://plugins.jetbrains.com/plugin/21289-aicommit)


https://github.com/AICommitApp/community/raw/main/.github/images/aicommit-video.mp4

Intelligent commit message writer powered by AI!

- Generating commit messages using OpenAI
- Supporting custom prompts and various parameter adjustments
- High integration with JetBrain products for an excellent user experience
- Putting privacy first by not collecting any code information
- We’ve incorporated a simple but effective algorithm for calculating JVM tokens to prevent hitting your token limit.
- For scenarios with a large number of changed files, the process is split and executed concurrently, resulting in blazingly fast speed.

## Installation

- Using IDE built-in plugin system:

  <kbd>Settings/Preferences</kbd> > <kbd>Plugins</kbd> > <kbd>Marketplace</kbd> > <kbd>Search for "AICommit"</kbd> >
  <kbd>Install Plugin</kbd>

## Configuring [OpenAI Token](https://platform.openai.com/account/api-keys)
In the AiCommit plugin, you'll need to enter your OpenAI access token to start using the plugin. At the top of the AiCommit window, enter your OpenAI access token. Then, click "Verify" to ensure your access token is valid.

## Getting Started
Once you have successfully installed the plugin and configured your OpenAI token, you're ready to start using AiCommit. You can now launch AiCommit on your current project and begin generating commit messages. Click the "Generate" button at the bottom of the window to create a commit message for your project.

## Roadmap

- [ ] Localize the plugin
- [ ] Commit Action with progress status.
- [ ] Generating commit information only for selected files.
- [ ] Supports filtering files or folders.
- [ ] Support for more commit message templates, prefixes, and suffixes.
- [ ] Support for code documentation generation
- [ ] Support for GPT-4 API

---

## Credit
- [AICommit](https://github.com/Nutlope/aicommits):A CLI that writes your git commit messages for you with AI. Never write a commit message again.
- [Openai-Kotlin](https://github.com/aallam/openai-kotlin): Kotlin client for OpenAI's API with multiplatform and coroutines capabilities.
- [java-diff-utils](https://github.com/java-diff-utils/java-diff-utils)
- Plugin based on the [IntelliJ Platform Plugin Template][template].
- Deja Vu by Cykarl https://soundcloud.com/cykarl
  Creative Commons — Attribution 3.0 Unported — CC BY 3.0
  Free Download / Stream: https://bit.ly/3IPXpnU
  Music promoted by Audio Library https://youtu.be/-tPlIz3eov4

[template]: https://github.com/JetBrains/intellij-platform-plugin-template
