## Policies

- Policies are lists of requirements for an authorization
- Requirements are data parameters which can be checked against when attempting an authorization
- Requirements are small classes which are instantiated when they are added to a policy
- This structure allows you to use the same requirement with different values for different policies
- Requirements of a policy are checked on authorization attempt by the `IAuthorizationService` interface
- Handlers for authorization are added to your configurations in `ConfigureServices()`
- Policies and policy requirements are added to your authorization via the authorizations options under `ConfigureServices()` via `options.AddPolicy()`
- For example:
```csharp
public void ConfigureServices(IServiceCollection services)
{
...
  services.AddAuthorization(options =>
  {
    options.AddPolicy("PolicyName", policy =>
      policy.Requirements.Add(new PolicyClassName(val)));
  });
...
}
```
- Policies are added to MVC controllers or Razor Pages with the attribute [Authorize(Policy = "PolicyName")] above the class declaration
