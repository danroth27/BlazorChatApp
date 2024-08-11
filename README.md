# BlazorChatApp

This is a simple AI-powered Blazor chat app that uses [Semantic Kernel](https://aka.ms/semantic-kernel) with a custom [plugin](https://learn.microsoft.com/semantic-kernel/concepts/plugins) to enable the AI assistant to change the theme colors of the app.

## Configure the Azure OpenAI backend

1. [Create and deploy an Azure OpenAI resource](https://learn.microsoft.com/azure/ai-services/openai/how-to/create-resource).

1. This app uses the [Azure Identity client library](https://learn.microsoft.com/dotnet/api/overview/azure/identity-readme) to authenticate with Azure OpenAI. Use [Role-based access control](https://learn.microsoft.com/dotnet/api/overview/azure/identity-readme) to grant permissions to the appropriate identity or group to have access to the Azure OpenAI resource.

1. Configure the deployment name and endpoint URL for your Azure OpenAI resource:

```json
{
  "SmartComponents": {
    "DeploymentName": <Azure OpenAI deployment name>,
    "Endpoint": <Azure OpenAI endpoint URL>
  }
}
```

1. Run the app and start chatting with the AI assistant. Try asking the AI assistant to change the theme colors of the app.
