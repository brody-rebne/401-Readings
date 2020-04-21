## Identity on ASP.NET Core

- ASP.NET Core Identity adds login functionality to .NET Core apps
- Allows for internal logins and/or external login providers
- Identity data can be stored in a SQL db or other storage services
- #### Creating authentication
  - Select an ASP.NET Core Web App, and select **Change Authentication**
  - Select **Individual User Accounts**
- #### Configuring Identities
  - Done in `ConfigureServices` method
  - Refer to [reading](https://docs.microsoft.com/en-us/aspnet/core/security/authentication/identity?view=aspnetcore-2.1&tabs=visual-studio#configure-identity-services-1) for configuration
- Identity services should be ready to scaffold into views and controllers
