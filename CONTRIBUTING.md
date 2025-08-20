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
- **Must**: Pull requests' code should be 100% related to the issue being solved. Anything unrelated should be moved into its own atomic PR
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

## AI Assistance Notice

We require disclosure of AI assistance in pull requests to maintain transparency and help reviewers understand the contribution process. This helps us:

- Understand the development process behind contributions
- Provide appropriate review and feedback
- Maintain code quality standards
- Build trust within our contributor community

### Disclosure Requirements

When submitting a pull request that involved AI assistance (such as GitHub Copilot, ChatGPT, Claude, or similar tools), please include a brief note in your PR description indicating:

1. **What AI tools were used** (if any)
2. **How they were used** (code generation, debugging, documentation, etc.)
3. **What portions of the contribution involved AI assistance**

### Examples

**Good disclosure examples:**
- "Used GitHub Copilot for boilerplate code generation in the new authentication module"
- "ChatGPT helped debug the memory leak in the connection pool implementation"
- "Claude assisted with writing unit tests for the new API endpoints"
- "No AI was used to generate any of this code"

**What doesn't need disclosure:**
- Standard IDE features (autocomplete, syntax highlighting, etc.)
- Search engines and documentation lookup
- Stack Overflow and similar Q&A sites

### Why We Ask

This policy isn't about restricting AI use—we recognize AI tools can be valuable development aids. Instead, it's about transparency and helping our maintainers provide the best possible review. Knowing how a contribution was developed helps us:

- Focus review attention appropriately
- Provide better feedback and mentorship
- Understand patterns in our codebase development
- Make informed decisions about our development practices

Thank you for helping us maintain a transparent and collaborative development environment!

## License

By contributing, you agree that your contributions will be licensed under the [MIT License](LICENSE.md).
