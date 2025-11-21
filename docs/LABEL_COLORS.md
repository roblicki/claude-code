# Label Organization Guide

## Label Categories

| Label Name | Category | Description |
|------------|----------|-------------|
| bug | issue-type | Something isn't working |
| enhancement | issue-type | New feature or request |
| documentation | issue-type | Improvements or additions to documentation |
| question | issue-type | Further information is requested |
| duplicate | status | This issue or pull request already exists |
| has repro | status | A reproducible case has been provided |
| external | status | Issue is caused by or tracked in an external dependency |
| area:core | area | Core CLI/runtime functionality |
| area:tools | area | Built-in tools (Read, Edit, Write, Search/Grep, Bash, etc.) |
| area:model | area | Model behavior, reasoning, or outputs |
| area:ide | area | IDE integration and plugins |
| area:tui | area | Terminal UI / interactive interface |
| area:mcp | area | Model Context Protocol servers and integrations |
| area:api | area | API layer, requests/serialization |
| area:auth | area | Authentication and credentials |
| area:packaging | area | Distribution, install, updating, packaging artifacts |
| area:security | area | Permissions, sandboxing, safety controls |
| platform:macos | platform | macOS-specific behavior |
| platform:linux | platform | Linux-specific behavior |
| platform:windows | platform | Windows-specific behavior |
| memory | performance | Memory usage or constraints |
| perf:memory | performance | Performance issues related to memory (heap, leaks, OOM) |

## Usage Guidelines

- Apply one issue-type label to indicate the nature of the ticket (bug, enhancement, documentation, question).
- Add one or more area labels to indicate the component involved (core, tools, model, IDE, TUI, MCP, API, auth, packaging, security).
- Use a platform label when the issue is specific to macOS, Linux, or Windows.
- Use status/triage labels to clarify current triage state:
  - has repro when a minimal reproducible example or clear steps exist.
  - duplicate when the issue tracks the same problem as another ticket; add a link to the original.
  - external when the cause lies in an upstream dependency or external system.
- Use performance labels when the problem primarily concerns resource usage or speed:
  - memory for general memory topics and constraints.
  - perf:memory for performance-impacting memory issues (heap/OOM/leaks).
- Prefer consistency: prioritize existing labels over creating new ones; propose new labels via PR if truly needed.
- Keep labels concise and avoid over-labeling: aim for an issue-type, 1–3 area labels, optional platform, and optional status/performance as appropriate.
