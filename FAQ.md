# AICommit FAQ

## Product and Usage Questions

1. **How does AICommit work?**
   AICommit uses JetBrains Platform's API to identify code changes and sends the changes to OpenAI's GPT model. It uses the GPT model to analyze the diff, which helps in automating the writing of commit messages.

2. **Will my code be exposed?**
   AICommit does not collect your code. The changes to your code (not the entire code) will be sent to OpenAI's API service, just like when you use ChatGPT. We suggest you read our user terms [here](https://github.com/AICommitApp/community/blob/main/EULA.md) and OpenAI's privacy terms [here](https://openai.com/policies/terms-of-use).

3. **Do I need to prepare my own OpenAI token?**
   Yes, you need to. You can obtain the token [here](https://platform.openai.com/account/api-keys). AICommit is dedicated to minimizing token consumption.

4. **Will my token be exposed?**
   No, AICommit will not collect your token. Your token will be sent only to OpenAI's API service. If you have set up a custom domain, the token will be sent to the domain for authentication.

## Common Issues

5. **Encountering 'ConnectException: Operation timed out' or 'SocketException: Connection reset'?**
   Check your network and proxy settings [here](https://www.jetbrains.com/help/idea/settings-http-proxy.html).

6. **Encountering 'Unknown error in verifyToken'?**
   An unexpected problem might have occurred. First, please update to the latest version. If the problem persists, please create an issue or contact us via email.

7. **Encountering 'You exceeded your current quota, please check your plan and billing details'?**
   Your OpenAI request hit the limit. Check the official documentation [here](https://help.openai.com/en/articles/6891831-error-code-429-you-exceeded-your-current-quota-please-check-your-plan-and-billing-details).

8. **Encountering 'Rate limit reached for default-gpt-3.5-turbo in organization...' ?**
   The model request has reached the limit. OpenAI limits API requests for users with different payment plans. Check [here](https://platform.openai.com/docs/guides/rate-limits#:~:text=Default%20rate%20limits%20for%20gpt,increases%20due%20to%20capacity%20constraints) for more information. We recommend waiting for 1 minute or changing to another model.

9. **Encountering 'SocketException: A connection attempt failed because the connected party did not properly respond after a period of time, or established connection failed because connected host has failed to respond'?**
   Network timeout, check your network and proxy settings [here](https://www.jetbrains.com/help/idea/settings-http-proxy.html).

10. **Encountering 'Invalid authorization header'?**
    Make sure your token is set and valid.

11. **Encountering 'That model is currently overloaded with other requests. You can retry your request, or contact us through our help center at help.openai.com if the error persists.'?**
    OpenAI hit the limit, check [here](https://community.openai.com/t/status-code-503-that-model-is-currently-overloaded-with-other-requests/31433).

12. **Encountering 'This model's maximum context length is 4097 tokens. However, you requested 4335 tokens (2970 in the messages, 1365 in the completion).'?**
    AICommit is optimizing the token calculation algorithm to address this issue soon.

13. **Encountering 'The server had an error while processing your request. Sorry about that!'?**
    OpenAI service hit the limit, check [here](https://community.openai.com/t/openai-api-error-the-server-had-an-error-while-processing-your-request-sorry-about-that/53263).
