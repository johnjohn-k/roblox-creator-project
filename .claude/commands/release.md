Prepare release checklist for: $ARGUMENTS

Process:
1. Review all code in `src/` for debug statements (print/warn in production paths)
2. Use `qa-tester` agent to confirm test checklist is complete
3. Run `codex:rescue` for final review of all changes since last release

Release checklist:
- [ ] No debug print/warn statements in production code paths
- [ ] All RemoteEvent/Function handlers have server-side validation
- [ ] DataStore error handling present
- [ ] QA test plan executed in Roblox Studio
- [ ] Codex final review complete
- [ ] All `src/` files have correct placement paths in comments
- [ ] Release notes written to `docs/tasks/YYYY-MM-DD-release.md`
- [ ] Changes committed and pushed to GitHub

Output: checklist status, any blocking issues, and recommended Studio publish order.
