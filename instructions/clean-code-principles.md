---
name: 'clean-code-principles'
description: 'Clean code principles and practices for PHP development'
---

# Clean Code Principles for PHP

## Naming Conventions
- Use descriptive and unambiguous names
- Use pronounceable and searchable names
- Avoid mental mapping and cryptic abbreviations
- Classes: PascalCase (e.g., UserRepository, OrderService)
- Methods/Functions: camelCase (e.g., getUserById, processPayment)
- Constants: UPPER_SNAKE_CASE (e.g., MAX_RETRY_COUNT)
- Variables: camelCase, descriptive (e.g., $userEmail, $totalAmount)

## Functions/Methods
- Keep functions small (ideally < 20 lines)
- Do one thing and do it well (Single Responsibility)
- Use descriptive names that reveal intent
- Limit function parameters (max 3-4, use objects for more)
- Avoid side effects and flag arguments
- Use type hints and return type declarations

## Classes
- Single Responsibility Principle: One reason to change
- Keep classes focused and cohesive
- Favor composition over inheritance
- Use dependency injection
- Apply SOLID principles
- Keep class size reasonable (< 300 lines)

## Comments
- Code should be self-documenting
- Use comments to explain "why", not "what"
- Keep comments up to date
- Use PHPDoc for public APIs
- Remove commented-out code

## Error Handling
- Use exceptions for exceptional cases
- Create custom exception classes
- Don't return null; use null object pattern or throw exceptions
- Validate input at boundaries
- Fail fast and provide meaningful error messages

## Code Organization
- Follow PSR-4 autoloading
- Group related functionality
- Separate concerns (controllers, services, repositories)
- Use meaningful directory structures
- Keep configuration separate from code
