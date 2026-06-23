---
name: Git Commit Summarizer
description: Analyzes git diffs and automatically generates concise, conventional commit messages when the user asks to "commit", "write a commit message", or asks "what did I change?"
---

## Git Commit Summarizer

This skill analyzes git diffs and generates concise, conventional commit messages. It helps software engineers and AI coding agents streamline their workflow by creating standardized commit descriptions.

### Workflow Steps

1. User triggers the skill by asking to commit or inquire about changes.
2. The skill retrieves the current git diff.
3. The skill analyzes the changes made in the git diff.
4. A conventional commit message is generated based on the analysis.
5. The skill outputs the commit message in a markdown code block.

### Output Format

The output will be a markdown code block containing a valid conventional commit message, such as:

```
feat: add login modal
```

### Examples

**Input:** "commit"  
**Output:**
```
fix: correct typo in README
```

**Input:** "what did I change?"  
**Output:**
```
refactor: update user model structure
```

### Anti-Patterns

- Do not generate commit messages longer than 50 characters for the first line.
- Avoid including detailed explanations or descriptions in the output.
- Do not create messages based on unrelated changes or files.

### Scope

The skill is aimed at software engineers and AI coding agents who need efficient commit message generation. Future enhancements may include support for custom commit message formats, integration with various version control systems, and the ability to learn from user preferences for commit messages.