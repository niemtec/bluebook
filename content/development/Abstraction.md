Abstraction is the act of dealing with "ideas" or higher-level functionality without knowing what the implementation will be.

- This is typically done by providing a public-facing interface that the code interacts with
- This hides implementation details and leaves your code only "knowing" about the function itself and what is expected from it

Abstraction is required when you want to decouple your implementation details from your application, doing so provides benefits:

- **Long-term maintenance is easier**: since business logic is written against interfaces (not the implementation) as long as the interfaces return the expected values you can change your implementations multiple times without having to refactor
- **Easier to understand**: it's a declarative approach leaving out implementation details, when you read declarative code you're reading what the code is doing, not how it's being done
- **Easier to test**: unit tests can be written against the interface, if you have a level of abstraction that allows you to supply Mock versions of fake data versions you can write more robust unit tests that cover a wider range of functionality
- **Fake Data**: you can set up and supply a fake data implementation of all your services (that are dependent on outside forces), you can even start developing your app before the API is complete and help define the responses the app requires to function
