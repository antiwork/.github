# Contributing to Antiwork Projects

## Commenting on GitHub

Use native-sounding English in all communication with no excessive capitalization (e.g HOW IS THIS GOING), multiple question marks (how's this going???), grammatical errors (how's dis going), or typos (thnx fr update).
- ❌ Before: "is this still open ?? I am happy to work on it ??"
- ✅ After: "Is this actively being worked on? I've started work on it here…"

Check existing discussions/issues/PRs before creating new ones. Start a discussion for questions or ideas.

## Issues

A great bug report includes:

- A quick summary and/or background
- Steps to reproduce
  - Be specific!
  - Give sample code if you can
- What you expected would happen
- What actually happens
- Notes (possibly including why you think this might be happening, or stuff you tried that didn't work)

We don't assign issues to contributors until they have a history of contributions to the project.

## Pull Requests (code)

### General best practices

1. Update documentation if you're changing behavior
2. Add or update tests for your changes
3. Include screenshots of your test suite passing locally
4. Make sure all tests pass
5. Request a review from maintainers
6. After reviews begin, avoid force-pushing to your branch
   - Force-pushing rewrites history and makes review threads hard to follow
   - Don't worry about messy commits - we squash everything when merging to main
7. Self-review your PR with explanatory comments for any non-intuitive or non-obvious changes to help reviewers understand your reasoning
8. The PR will be merged once you have the sign-off of at least one other developer

### Front-end

- Follow the existing code patterns
- Use clear, descriptive variable names
- Write TypeScript for all code
- Follow Next.js and React conventions

### Back-end

- Follow the existing code patterns
- Use clear, descriptive variable names
- Write TypeScript for all code
- Use Prisma best practices for database operations

### TypeScript and React Guidelines

- Write TypeScript for all code
- Follow React best practices and use functional components
- Use lowerCamelCase for component file names (e.g., `conversationList.tsx`)
- Design for both light and dark mode
- Consider mobile and desktop devices (medium, large, and extra large breakpoints)
- No explanatory comments unless explicitly needed

### Testing Guidelines

- Write descriptive test names that explain the behavior being tested
- Keep tests independent and isolated
- For API endpoints, test response status, format, and content
- Use factories for test data instead of creating objects directly
- Test both happy path and edge cases
- Use Vitest for unit tests and Playwright for end-to-end tests
- Fix existing tests if required, but don't add new tests unless explicitly told to do so

### Monorepo Structure

When working with monorepo projects:
- Use pnpm workspaces for package management
- Refer to individual package CONTRIBUTING.md files for package-specific guidelines
- Follow existing code patterns within each package

### Development Practices

- Don't modify config files or package.json unless explicitly told to do so
- Use clear, descriptive variable names
- Follow existing code patterns in the repository

## License

By contributing, you agree that your contributions will be licensed under the [MIT License](LICENSE.md).
