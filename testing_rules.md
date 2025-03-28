# Testing Rules

## 1. Test Coverage

- Aim for high test coverage of code, but focus on coverage of functionality
- Test edge cases and boundary conditions
- Include negative testing (invalid inputs, error conditions)
- Test both happy paths and failure scenarios
- Ensure all critical paths have thorough test coverage

## 2. Test Organization

- Structure tests logically to match application organization
- Use descriptive test names that indicate what is being tested
- Group related tests together
- Separate unit tests from integration and system tests
- Follow a consistent naming convention for test files and functions

## 3. Test Independence

- Each test should be independent and self-contained
- Tests should not depend on the order of execution
- Avoid test interdependencies
- Reset the test state between test runs
- Mock external dependencies to ensure test isolation

## 4. Test Quality

- Tests should be deterministic (same result every time)
- Avoid flaky tests that pass/fail inconsistently
- Keep tests simple and readable
- Tests should run quickly to enable frequent execution
- One assertion per test is ideal (or testing one logical concept)

## 5. Test Maintenance

- Treat test code with the same care as production code
- Refactor tests when they become difficult to maintain
- Avoid duplicated test code using appropriate abstractions
- Keep test fixtures and helpers up to date
- Delete tests that no longer serve a purpose

## 6. Regression Testing

- Automate regression tests wherever possible
- Create tests for all reported bugs to prevent recurrence
- Run regression tests before each release
- Prioritize tests based on risk and importance
- Include visual regression tests for UI components

## 7. Non-Functional Testing

- Test performance under expected and peak loads
- Test security aspects including authentication and authorization
- Validate accessibility compliance
- Test internationalization and localization
- Test compatibility with supported browsers/devices/platforms

## Testing Phase Focus Tips

- Write tests before or alongside code (TDD/BDD) when appropriate
- Automate tests within CI/CD pipelines
- Use appropriate testing frameworks for different test types
- Review test reports and address failures promptly
- Consider mutation testing to validate test effectiveness
- Document the test strategy and approach for the project 