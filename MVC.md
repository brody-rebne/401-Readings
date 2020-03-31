## MVC

- Model-View-Controller
- Architectural pattern for separation of concerns in an app
- Model:
  - The state of the applications data
  - Updated by the Controller
  - Updates the data for the View
  - "Business Logic"
- View:
  - Presentation layer
  - User-facing content of the app
  - Updated by Model
  - Sends requests via Controller
  - Minimal logic only for presentation
- Controller:
  - Handles requests and input from user
  - Renders the View
  - Sends requests to Model
  - Redirects to proper View/Model based on task

## ASP.NET Core MVC:
- Build on URL-mapping system
- Defines naming patterns for URLs
- Good for SEO
- Dynamically generate links without managing file structure
- Received requests are mapped to defined URL formats
