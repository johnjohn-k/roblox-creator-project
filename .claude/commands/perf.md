Use the `perf-optimizer` agent to analyze performance for: $ARGUMENTS

If no target is specified, audit all scripts in `src/` for common performance issues.

Process:
1. Scan source files for known anti-patterns (loop instantiation, unbounded connections, high-frequency remotes)
2. Prioritize issues by impact (frame time / server load)
3. Propose concrete fixes with expected improvement
4. Run `codex:rescue` to validate proposed changes

Output: issues ranked by severity, fix proposals with code examples, estimated performance gain.
