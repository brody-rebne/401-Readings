## Razor Pages

- Razor Pages is a newish functionality of ASP.NET Core MVC that allows you to build page-focused apps in a more straightforward and simpler manner
- They handle https requests directly, instead of needing a controller
- They can be loaded by name more easily, instead of manually pairing routes with filepaths
- By virtue of these two benefits, they are very useful in smaller-scoped apps with less need for rock-solid and partitioned architecture
- They are also much easier to understand at their core than the disparate and unnaturally syntaxed traditional MVC methods
- I love razor pages!
- Razor Pages are also built syntactically off of Razor views, which many (including us) are already familiar with
- Pages require a `@page` directive, the most important element of their functionality
- This directive turns the page into an MVC action, which allows it to bypass its otherwise necessary controller
- Pages come with an attached model, named `filename.cshtml.cs`
- This model is what contains the functionality required on http requests
- Functionality is given inside of `OnGet()`/`OnPost()` (or `OnGetAsync()`/`OnPostAsync()`) methods within this model
