## User Secrets

- Secure way of storing private user information
- Types of private info can include API keys, client secrets, and connection strings
- To enable user secrets in Visual Studio:
  - Right click on project file and click Manage User Secrets
    - File built to house user secrets in JSON will open
    - Add any user secrets as key value pairs here
    - File will not be pushed to source control, or even be stored in local repo
  - Then go to your .csproj file
    - User secrets file ID will be auto-added
    - Add the line `<DotNetCliToolReference Include="Microsoft.Extensions.SecretManager.Tools" Version="2.0.0" />` to the file (trust the system)
  - User secrets will now be enable and available for access within the project
- You will then need to:
  - Create a configuration builder within startup file
  - Bring in the configuration to startup file
  - Pass the configuration to your controller constructor (dependency injection!)
  - Update your Azure deployment to use the user secrets configuration
  - Reference the [Reading](https://codefellows.github.io/code-401-dotnet-guide/Resources/UserSecrets.html) for this process and syntax
  
