### Directory Structure

```txt
/tests
│
├── /unit # Unit tests for individual components
│ ├── /core # Unit tests for the core domain logic
│ │ └── UserService.test.ts
│ ├── /application # Unit tests for the application layer
│ │ └── CreateUserUseCase.test.ts
│ ├── /infrastructure # Unit tests for the infrastructure layer
│ │ ├── /database # Unit tests for database implementations
│ │ │ └── UserRepositoryImpl.test.ts
│ │ ├── /services # Unit tests for external services
│ │ │ └── EmailService.test.ts
│ │ └── /adapters # Unit tests for adapters
│ │ └── S3Adapter.test.ts
│ └── /presentation # Unit tests for the presentation layer
│ ├── /rest # Unit tests for RESTful API
│ │ └── UserController.test.ts
│ ├── /graphql # Unit tests for GraphQL API
│ │ └── UserResolver.test.ts
│ └── /cli # Unit tests for CLI commands
│ └── CreateUserCommand.test.ts
│
├── /integration # Integration tests for testing how components interact
│ └── CreateUserIntegration.test.ts
│
└── /e2e # End-to-end tests (e.g., API testing, UI testing, CLI testing)
└── UserE2ETest.ts
```
