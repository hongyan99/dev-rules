# Implementation Phase Rules

## 1. API Consistency

- Maintain the same parameter names and types in interface implementations
- Keep response format consistent between implementations of the same interface
- Implement all required methods from base classes in all derived classes
- Follow established patterns within the codebase

## 2. Documentation

- Update docstrings when implementing methods
- Include type hints for all method parameters and return values
- **NEVER** remove existing comments unless they are factually incorrect
- Add comprehensive comments for complex logic or non-obvious decisions
- Document edge cases and how they're handled

## 3. Implementation Simplicity

- Keep implementations as simple as possible without sacrificing functionality
- Avoid clever/complex solutions when simpler ones will suffice
- Prefer readability and maintainability over premature optimization
- Follow the principle of least surprise in your implementations
- Don't over-engineer: implement what's needed now, not what might be needed later
- Document any necessarily complex implementations thoroughly

## 4. Error Handling and Logging

- Add appropriate logging for initialization and external service calls
- Include informative error messages with potential resolution steps
- Handle all expected exceptions and log appropriate context
- Don't swallow exceptions without proper handling
- Use structured logging where appropriate

## 5. Security Considerations

- **NEVER** weaken security controls during implementation
- Be extremely cautious when implementing authentication, authorization, or encryption
- Maintain or improve input validation and output encoding
- Consider potential injection vulnerabilities in your code
- Apply the principle of least privilege

## 6. Dynamic Loading

- Keep imports inside methods when implementing dynamic loading pattern
- Only load dependencies when actually needed (lazy loading)
- Provide clear error messages when optional dependencies are missing

## Implementation Phase Focus Tips

- Follow established coding standards and patterns
- Write comprehensive unit tests alongside implementation
- Use meaningful variable and function names
- Implement error handling and validation robustly
- Keep functions small and focused on a single responsibility
- Use appropriate data structures for the task
- Consider thread safety if applicable 