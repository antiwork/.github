# Contributing to Antiwork Projects

Respect others by using professional, easy-to-read English that transcends cultures.

That means no excessive capitalization (e.g HOW IS THIS GOING), multiple question marks (how's this going???), grammatical errors (how's dis going), or typos (thnx fr update).

## Issues

We don't assign issues to contributors until they have a history of contributions to the project. Even then, assignments are rare.

## Pull Requests (code)

Pull Requests should close open issues.

Please include an AI disclosure as well as a confirmation you've watched our [PR live streaming videos](https://www.youtube.com/@anti-work).

### General best practices

- Update documentation as you go
- Add or update tests for your changes–any functional changes should reflect in updated/new end-to-end tests
- Include screenshots of your test suite passing locally if the build doesn't run automatically
- Make sure **all** tests pass
- Request a review from one maintainer
- After reviews begin, avoid force-pushing to your branch
   - Force-pushing rewrites history and makes review threads hard to follow
   - Don't worry about messy commits - we squash everything when merging to main
- **Must**: Self-review your PR with explanatory comments for any non-intuitive or non-obvious changes to help reviewers understand your reasoning
- **Must**: Code should be 100% related to the issue being solved. Anything unrelated should be moved into its own atomic PR
- **Must**: Contain videos of before/after with light/dark mode and mobile/desktop represented 
- Newlines at end of files

### Front-end

- Follow the existing code patterns
- Use clear, descriptive variable names
- Write TypeScript for all code
- Follow Next.js and React conventions
- Use UpperCamelCase for component file names (e.g., `ConversationList.tsx`)
- Always use the latest version of TypeScript, React, and Next.js
- Use sentence case headers and buttons, not title case (Add board is good, Add Board is bad)
- When creating new components using Shadcn, use the `canary` version over the `latest` version

### Back-end

- Follow the existing code patterns
- Use clear, descriptive variable names
- Write tests for new methods, controllers, etc

### Design / UX

- Design for both light and dark mode
- Design for mobile and desktop

### Testing Guidelines

- Write descriptive test names that explain the behavior being tested
- Keep tests independent and isolated
- For API endpoints, test response status, format, and content
- Use factories for test data instead of creating objects directly
- Test both happy path and edge cases

## AI Assistance Notice

> [!IMPORTANT]
>
> If you are using **any kind of AI assistance** to contribute to Antiwork,
> it must be disclosed in the pull request with specific details.

If you are using any kind of AI assistance while contributing to Antiwork,
**this must be disclosed in the pull request**. Your disclosure must include:

1. **The specific AI model/tool used** (e.g., "Claude 3.5 Sonnet", "GPT-4", "GitHub Copilot", "Cursor", "Claude Code", etc.)
2. **Which tasks used AI assistance:**
   - Codebase exploration/understanding
   - Code generation
   - Debugging
   - Test writing
   - Documentation
   - PR description generation
   - Other (specify)
3. **Any IDE plugins or tools** (e.g., "Cursor", "GitHub Copilot", "Continue")

As a small exception, trivial tab-completion doesn't need to be disclosed,
so long as it is limited to single keywords or short phrases.

### Example disclosures

✅ **Good disclosure:**

> **AI Disclosure**
> - Model: Claude 3.5 Sonnet via Cursor
> - Used for: Codebase exploration, understanding existing patterns, and generating initial test structure
> - Code was manually reviewed and modified by me

✅ **Good disclosure:**

> **AI Disclosure**
> - Model: GPT-4 via ChatGPT
> - Used for: Understanding the authentication flow only
> - All code written manually by me

❌ **Insufficient disclosure:**

> AI assistance was used for understanding the codebase structure and implementing the feature according to existing patterns.

(Missing: specific model, unclear which tasks, no mention of tools)

❌ **Insufficient disclosure:**

> This PR was written primarily by Claude Code.

(Missing: specific model version, no task breakdown)

### No AI disclosure

If no AI assistance was used, please state explicitly:

> No AI was used for any part of this contribution.

Please be respectful to maintainers and provide complete AI disclosures.

## License

By contributing, you agree that your contributions will be licensed under the [MIT License](LICENSE.md).
