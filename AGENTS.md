# cloud-computing Development Guidelines

> A plain-language glossary of cloud computing, AI/ML, data, and infrastructure terms.

## Project Overview

cloud-computing is a documentation-only repository written in Markdown. The whole
glossary lives in `README.md`: 153 terms grouped under seven topic headings, with the
same content mirrored as a JSON block at the end of that file. There is no build step,
no dependency install, and no test suite. To validate a change, confirm the JSON block
still parses and that every entry in it has a matching `###` heading above.

### Terminal Management

- **Always use background terminals** (`isBackground: true`) for every command so a terminal ID is returned
- **Always kill the terminal** after the command completes, whether it succeeds or fails — never leave terminals open
- Do not reuse foreground shell sessions — stale sessions block future terminal operations in Codespaces
- In GitHub Codespaces, agent-spawned terminals may be hidden — they still work. Do not assume a terminal is broken if you cannot see it
- If a terminal appears unresponsive, kill it and create a new one rather than retrying in the same terminal

## Contributing

- Follow the existing code style
- Test changes before submitting PRs
- Update documentation when adding features
- See [CONTRIBUTING.md](CONTRIBUTING.md) for full guidelines
