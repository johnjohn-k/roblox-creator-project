Use the `luau-developer` agent to generate or review Luau code for: $ARGUMENTS

Output rules:
- Always include placement path at the top: `-- 配置先: [ServiceName]/[Path]/[FileName].luau`
- Use strict Luau type annotations
- Server-side validation on all RemoteEvent/Function handlers (never trust client)
- Wrap DataStore calls in pcall with retry logic

Review checklist:
- [ ] Security: server-side validation present, no client trust
- [ ] Performance: no instance creation in loops, connections cleaned up
- [ ] Error handling: pcall on DataStore/network calls
- [ ] Types: strict Luau annotations present
- [ ] Placement path clearly stated

Always run `codex:rescue` for a mandatory second-opinion pass before presenting the final code.
Present: generated/reviewed code block, placement path, and any caveats for Studio setup.
