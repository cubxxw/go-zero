```markdown
# go-zero Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill teaches the core development patterns and conventions used in the `go-zero` repository, which is primarily written in TypeScript and utilizes Go as its backend framework. You'll learn about file organization, code style, commit practices, and how to write and structure tests in this codebase.

## Coding Conventions

### File Naming
- Use **camelCase** for file names.
  - Example: `userService.ts`, `orderHandler.ts`

### Import Style
- Use **relative imports** for modules within the project.
  - Example:
    ```typescript
    import { getUser } from './userService';
    ```

### Export Style
- Use **named exports** for functions, classes, and constants.
  - Example:
    ```typescript
    export function getUser(id: string) { ... }
    export const DEFAULT_TIMEOUT = 5000;
    ```

### Commit Patterns
- Follow **Conventional Commits**.
- Common prefix: `chore`
- Keep commit messages concise (average ~33 characters).
  - Example:
    ```
    chore: update dependencies
    ```

## Workflows

_No automated or CI workflows were detected in this repository._

## Testing Patterns

- Test files follow the pattern: `*.test.*`
  - Example: `userService.test.ts`
- The specific testing framework is unknown, but tests are colocated with source files or in dedicated test files.
- Example test file structure:
  ```typescript
  // userService.test.ts
  import { getUser } from './userService';

  describe('getUser', () => {
    it('should return user data', () => {
      // test implementation
    });
  });
  ```

## Commands
| Command | Purpose |
|---------|---------|
| /commit-convention | Show commit message guidelines |
| /test-patterns     | Show test file naming and structure |
| /code-style        | Show code style conventions        |
```