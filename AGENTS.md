# Documentation project instructions

## About this project

- This is the Chinese user documentation for SDLC Harness.
- The site is built with Mintlify. Pages are MDX files with YAML frontmatter.
- Configuration and navigation live in `docs.json`.
- Write for developers and coding-agent users, not internal maintainers.

## Terminology

- Use “功能” for feature and keep literal JSON values such as `passing` in code formatting.
- Use “审核” for governance validation, “验证” for executing a feature's verification commands, and “证据” for persisted evidence.
- Keep command names, file names, JSON fields, status values, owner, claim, workspace, worktree and ADR in code formatting or their established technical form.
- Refer to the product as “SDLC Harness” in prose and `sdlc-harness` in commands.

## Style preferences

- Use active voice and address the reader as “你”.
- Lead with what the command or result means, then explain details.
- Keep sentences concise and use sentence case for headings.
- Show runnable commands and realistic outputs.
- Explicitly distinguish `verify`, `validate`, and `provider github check` conclusions.

## Content boundaries

- Document released, user-facing behavior that is supported by the CLI and repository templates.
- Do not present planned commands or internal implementation helpers as available features.
- Do not claim that SDLC Harness proves requirement correctness or replaces a test framework, coding Agent, or project management system.
