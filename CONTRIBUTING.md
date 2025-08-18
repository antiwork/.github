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

- Update documentation if you're changing behavior
- Add or update tests for your changes–any functional changes should reflect in updated/new end-to-end tests
- Include screenshots of your test suite passing locally if the build doesn't run automatically
- Make sure **all** tests pass
- Request a review from one maintainer
- After reviews begin, avoid force-pushing to your branch
   - Force-pushing rewrites history and makes review threads hard to follow
   - Don't worry about messy commits - we squash everything when merging to main
- **Must**: Self-review your PR with explanatory comments for any non-intuitive or non-obvious changes to help reviewers understand your reasoning
- Newlines at end of files, always

### Front-end

- Follow the existing code patterns
- Use clear, descriptive variable names
- Write TypeScript for all code
- Follow Next.js and React conventions
- Use UpperCamelCase for component file names (e.g., `ConversationList.tsx`)
- Always use the latest version of TypeScript, React, and Next.js
- Use sentence case headers and buttons, not title case (Add board is good, Add Board is bad)
- Do not use `React.FC`. Use the following syntax: `const Component = ({ prop1, prop2 }: { prop1: string; prop2: number }) => { ... }`
- When building UI, use existing components from `components/` when available: `Button`, `Input`, `DataTable`, `Placeholder`, `ComboBox`, `NumberInput`, `MutationButton`, `Dialog`, `Form` components, etc.
- When creating new components using Shadcn, use the `canary` version over the `latest` version

### Back-end

- Follow the existing code patterns
- Use clear, descriptive variable names
- Write TypeScript for all code
- Use Prisma best practices for database operations
- Any changes to the back-end database schema must be reflected in any existing frontend schema files for type safety

### Design / UX

- Design for both light and dark mode
- Consider mobile and desktop devices (small, medium, large, and extra large breakpoints)
- Forms for adding new objects to the database should inherit values from the last object added to the table

### Testing Guidelines

- Write descriptive test names that explain the behavior being tested
- Keep tests independent and isolated
- For API endpoints, test response status, format, and content
- Use factories for test data instead of creating objects directly
- Test both happy path and edge cases

## License

By contributing, you agree that your contributions will be licensed under the [MIT License](LICENSE.md).
