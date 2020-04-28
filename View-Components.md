## View Components

- Similar to a partial view
- Work with both Razor Pages and views
- Contains business logic
- Maintains separation of concerns
- Allows use of parameters and business logic
- Good for things like:
  - Logins
  - Carts
  - Recent blog posts
- Split into two parts:
  - Class - contains logic
  - Result - contains code for rendering content
- Designating view components:
  - Method 1: deriving the class from the ViewComponent class
  - Decorating the class with [ViewComponent]
  - Creating a class with the suffix ViewComponent (unreliable)
- Support dependency injection
