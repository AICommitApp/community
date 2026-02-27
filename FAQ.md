# AICommit FAQ

## Product and Usage Questions

1. **What does AICommit do?**  
   AICommit analyzes staged changes in JetBrains IDEs and generates commit messages. You can insert the generated result directly into the Commit panel.

2. **Which AI providers are supported?**  
   OpenAI, Azure OpenAI, Google Gemini, Anthropic Claude, and Ollama (local models).

3. **What is PromptLab?**  
   PromptLab is the commit-prompt workspace in AICommit. You can choose built-in templates, edit custom prompts, save templates, set a default template, and include recent commit summaries as context.

4. **Do I need to provide my own API key?**  
   For cloud providers (OpenAI, Azure OpenAI, Gemini, Claude), yes. For Ollama, configure your local Ollama endpoint and model.

5. **Will AICommit collect my code or commit messages?**  
   AICommit does not collect your code or commit messages. Content is sent only to the provider you configured for generation. See [Privacy Policy](./PRIVACY_POLICY.md) and [EULA](./EULA.md).

6. **Can I run AICommit in a local-only mode?**  
   Yes. Use Ollama with local models for a local-first workflow.

7. **How do I get started quickly?**  
   Install the plugin, configure a provider and model, verify credentials, select a PromptLab template (or custom prompt), then click Generate.

## Common Issues

8. **`API key missing`, `verify token failed`, or provider activation failed**  
   Open AICommit settings and check key/endpoint/model for the selected provider. Re-run verification after saving settings.

9. **`No enabled models for <provider>`**  
   Go to settings and enable at least one model for the current provider.

10. **Network timeout / connection reset / SSL errors**  
   Check your network and proxy configuration in JetBrains: [HTTP Proxy Settings](https://www.jetbrains.com/help/idea/settings-http-proxy.html). Also verify your provider endpoint is reachable.

11. **Quota/rate-limit errors (`429`)**  
   Your provider quota or rate limit was reached. Wait and retry, switch to another model, or use another provider.

12. **Service overloaded / unavailable (`5xx`)**  
   The provider service is temporarily unavailable. Retry later or switch provider/model.

13. **`Invalid authorization header` or `Incorrect API key provided`**  
   Replace the key with a valid one for the selected provider and verify again.

14. **Azure: `The API deployment for this resource does not exist`**  
   Check Azure endpoint, deployment name, API version, and resource region. If you just created the deployment, wait a few minutes and retry.

15. **Generated result was copied to clipboard instead of inserted into Commit panel**  
   AICommit falls back to clipboard when it cannot find a writable Commit panel in the current context. Open/focus the Commit tool window and insert again.

16. **Prompt/template changes did not take effect**  
   Make sure the expected template is selected, save template changes, and set it as default if needed.

17. **`License is not valid`**  
   Check your plugin subscription/license status in JetBrains Marketplace and your IDE account.

18. **How do I report a bug?**  
   Please open an issue with IDE version, AICommit version, provider, model, and full error message: [Issue Tracker](https://github.com/AICommitApp/community/issues).
