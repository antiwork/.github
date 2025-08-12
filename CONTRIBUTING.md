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
- Always use the latest version of TypeScript, React, and Next.js
- Use sentence case headers and buttons, not title case
- Do not use `React.FC`. Use the following syntax: `const Component = ({ prop1, prop2 }: { prop1: string; prop2: number }) => { ... }`
- When building UI, use existing components from `components/` when available: `Button`, `Input`, `DataTable`, `Placeholder`, `ComboBox`, `NumberInput`, `MutationButton`, `Dialog`, `Form` components, etc.
- When creating new components using Shadcn, use the `canary` version over the `latest` version
- Add page to `app/**/page.tsx`
- Add any components to `components/**/*.tsx`
- Add tRPC API routes to `trpc/routes/**/index.ts` and then add those to `trpc/server.ts`
- Forms for adding new objects to the database should inherit values from the last object added to the table
- Newlines at end of files, always
- Add explanatory comments for race conditions and other unintuitive coding patterns

### Back-end

- Follow the existing code patterns
- Use clear, descriptive variable names
- Write TypeScript for all code
- Use Prisma best practices for database operations
- Any changes to the back-end database schema must be reflected in any existing frontend schema files for type safety

## License

By contributing, you agree that your contributions will be licensed under the [MIT License](LICENSE.md).
