# Antigravity Tool Mapping

This map translates Superpowers-standard workflow tools to Antigravity-native tools.

| Superpowers Tool | Antigravity Equivalent | Notes |
|------------------|------------------------|-------|
| `Skill`          | `view_file`            | Read `skills/<name>/SKILL.md` |
| `TodoWrite`      | `task_boundary` + `task.md` | Use `task_boundary` for UI, `task.md` for persistence |
| `Task`           | `task_boundary` update | Update the current task status and summary |
| `Task` (subagent)| `browser_subagent` / `run_command` | Subagents MUST inherit the "Superpowers grounding" - include specific skill instructions in their task description. |
| `Read`           | `view_file` / `list_dir` | Standard filesystem tools |
| `Write` / `Edit` | `multi_replace_file_content` | Use the most precise editing tool available |
| `Bash`           | `run_command`          | Execute in terminal |
| `Notify`         | `notify_user`          | Communicate with human partner |

## Usage Pattern

When a skill says:
> "Use `TodoWrite` to create a new task list"

You should:
1. Create/Update `<brain-dir>/task.md` (where `<brain-dir>` is your session's persistent context directory).
2. Call `task_boundary` with the `TaskName` corresponding to the first item.
