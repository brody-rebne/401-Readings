## LINQ

- Language INtegrated Query
- LINQ builds data queries directly into C#
- In other languages like JS, queries are dumb strings that are passed to the database blindly
- This prevents them from being typechecked or supported by IntelliSense
- Each data source's language must be studied and used depending on the target of the query
- LINQ in C# is a first-class construct
- Provides language-neutral, built-in (and thus IntelliSensed) syntax for queries
- Saves code as it implements query functionality into the code
-  Works on:
  - SQL Databases
  - ADO .NET Datasets
  - XML Docs/Streams
  - .NET Collections
  - Any collection of objects which support `IEnumerable`
- Can be used to convert data between languages
- Easier to parse and learn because syntax resembles C#
- Strongly typed, but types can be inferred (more on this?)

## LINQ Queries

- Three parts:
  - Obtain data source
  - Create query
  - Execute query
- This resembles steps we followed in a clinkier fashion using JS
- The query variable does not inherently contain or retrieve the data, it must be actually executed and request data from the source
