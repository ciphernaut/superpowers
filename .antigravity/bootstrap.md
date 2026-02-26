# Antigravity Protocol

When Superpowers is active, the Antigravity agent follows this protocol for optimal context management.

## Grounding Rules
1. **Skill First**: If a skill might apply, read its `SKILL.md` before any action or clarification.
2. **Persistence**: Use `task_boundary` for the UI and update `<brain-dir>/task.md` after every logical step.
3. **Verification**: Always provide terminal evidence or validation results before claiming a task is done.
4. **Native Tools**: Interpret Superpowers tool instructions (e.g., "Use Bash") as invitations to use your native Antigravity tools (`run_command`, `notify_user`, etc.).

Detailed templates and tool mappings are available in [ANTIGRAVITY.md](file:///projects/antigravity/superpowers/docs/ANTIGRAVITY.md).
