# AICommit

[![Version](https://img.shields.io/jetbrains/plugin/v/app.aicommit.plugin.svg)](https://plugins.jetbrains.com/plugin/app.aicommit.plugin)
[![Downloads](https://img.shields.io/jetbrains/plugin/d/app.aicommit.plugin.svg)](https://plugins.jetbrains.com/plugin/app.aicommit.plugin)


[![AI Commit](./assets/social_preview.jpg)](https://youtu.be/sDG8cx6i_kM "AI Commit")

智能提交信息撰写器，由AI提供动力！

- 使用OpenAI生成提交信息
- 支持定制提示和各种参数调整
- 与JetBrain产品高度集成，为用户带来出色的用户体验
- 通过不收集任何代码信息来保护隐私
- 我们使用简单而有效的算法来计算JVM令牌，以避免达到令牌限制。
- 对于有大量更改文件的情况，进程会被拆分并同时执行，为您带来极快的速度。

## 安装

- 使用IDE内置插件系统：

  <kbd>设置/首选项</kbd> > <kbd>插件</kbd> > <kbd>市场</kbd> > <kbd>搜索 “AICommit”</kbd> >
  <kbd>安装插件</kbd>

## 配置 [OpenAI Token](https://platform.openai.com/account/api-keys)

在 AiCommit 插件中，您需要输入 OpenAI 访问令牌以开始使用该插件。在 AiCommit 窗口的顶部，输入您的 OpenAI 访问令牌。然后，单击“验证”以确保您的访问令牌有效。

## 入门

安装了插件并成功配置了您的 OpenAI 令牌后，您就可以开始使用 AiCommit。您现在可以在当前项目上启动AiCommit并开始生成提交信息。单击窗口底部的“生成”按钮以为您的项目创建提交信息。

## 路线图

- [ ] 本地化插件
- [ ] 带有进度状态的提交操作。
- [ ] 仅针对选定文件生成提交信息。
- [ ] 支持过滤文件或文件夹。
- [ ] 支持更多的提交信息模板，前缀和后缀。
- [ ] 支持代码文档生成
- [ ] 支持GPT-4 API

---

## 信用

- [AICommit](https://github.com/Nutlope/aicommits)：一款使用AI为您编写Git提交信息的CLI。再也不用编写提交信息。
- [Openai-Kotlin](https://github.com/aallam/openai-kotlin)：具有多平台和协程功能的OpenAI API的Kotlin客户端。
- [java-diff-utils](https://github.com/java-diff-utils/java-diff-utils)
- 基于[ JetBrains平台插件模板][template]的插件。
- Deja Vu by Cykarl https://soundcloud.com/cykarl
  Creative Commons — Attribution 3.0 Unported — CC BY 3.0
  Free Download / Stream: https://bit.ly/3IPXpnU
  Music promoted by Audio Library https://youtu.be/-tPlIz3eov4

[template]: https://github.com/JetBrains/intellij-platform-plugin-template