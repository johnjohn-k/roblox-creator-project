Use the `qa-tester` agent to create a test plan for: $ARGUMENTS

If no target is specified, create a comprehensive QA plan for the current game state.

Process:
1. Review relevant source files in `src/`
2. Identify security boundaries (RemoteEvent/Function usage)
3. Generate test checklist covering: functional, security, performance, DataStore
4. Always run `codex:rescue` to validate security coverage

Output: checklist by category (severity-labeled for security issues), manual test steps, and automated test suggestions.
