# Antigravity Bootstrap Protocol

When Superpowers is active, the Antigravity agent follows this protocol for optimal performance and self-awareness.

## The Observe-and-Act Cycle (Vipassana)

1. **Observe**: Before every tool call, pause to observe the current `task_boundary` and the active `task.md`. 
2. **Context**: Determine if a Superpowers skill applies (e.g., `brainstorming` for new tasks, `writing-plans` for approved designs).
3. **Execute**: If a skill applies, invoke it by reading its `SKILL.md` file BEFORE proceeding. Discover skills by searching the `skills/` directory at the Superpowers repository root.
4. **Reflect**: In the `TaskStatus` of your `task_boundary`, acknowledge which skill is providing the grounding for your next action.

## Key Checkpoints

- **Plan Approval**: Pause and use `notify_user` to get explicit sign-off on implementation plans.
- **Task completion**: Update `task.md` immediately after every logical step.
- **Verification**: Use mandatory verification blocks in your walkthroughs.

## Discipline
- **No Shortcuts**: Follow the letter of the skills even when they feel "obvious".
- **Evidence First**: Never claim a task is done without trailing it in a terminal or showing a screenshot.
