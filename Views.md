## Views

### Layouts

- Layout files define pieces of front-end content to be easily re-used throughout an app
- Built in .cshtml files, often as `Pages/Shared/_Layout.cshtml` (Razor Pages) or `Views/Shared/_Layout.cshtml` (views for controller)
- The layout defines a base template for views
- Can be more than one layout file, for apps with multiple base layouts
- Layout files can bring in other .cshtml files as partials
- Sections allow small portions of code to be organized more easily
- Sections are defined via `@section SectionName { <div>You can put any amount of html here</div> }
- Sections can be called via `@RenderSections("SectionName", required: false)`
- Exception is thrown if required section is not found
- Namespaces can be imported to any view via a `_ViewImports.cshtml`
- They are imported via directives including `@using`, `@inherits`, and `@model`
