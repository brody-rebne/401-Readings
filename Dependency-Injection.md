## Dependency Injection

- Design pattern built to allow classes (usually controllers specifically) to require other objects
- This allows classes and objects to require very specific criteria, while remaining open-ended for flexible implementation
- Often dependencies are built on interfaces, which allows a broad range of objects to be passed in, but which all contain necessary functionality
- Often dependencies can be chained, to ensure a strong structure of reliance

## SOLID Principles

- Single Responsibility
  - Each method or class should have one single purpose/job/task within your app
- Open/Close
  - Each method or class should be open to extension, but closed to modification
  - Extension = improvements, new versions. Should be extended to improve functionality
  - Modification = changing existing versions. Should be left alone to maintain legacy versions' functionality
- Liskov Substitution
  - An object in use should be able to be replaced by a object derived from it, without breaking the application
- Interface Segregation
  - User interfaces should be purpose-built and targeted, so that users are not forced to go through steps which do not benefit them directly
- Dependency Inversion
  - Code should depend on abstract versions of things, instead of on the things themselves
  - This allows the code to continue functioning if the thing is replaced, without significant overhaul
