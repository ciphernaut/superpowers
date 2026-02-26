# Installing Superpowers for Antigravity

Antigravity natively utilizes Superpowers skills by symlinking them into the local environment and following the "Antigravity Protocol".

## Installation Steps

### 1. Symlink Skills
Create a symlink so Antigravity's tools can discover the skills:

```bash
mkdir -p ~/.agents/skills
ln -s "$(pwd)/skills" ~/.agents/skills/superpowers
```

### 2. Register Bootstrap Workflow
Register the superpowers workflow to enable automatic context injection:

```bash
mkdir -p .agents/workflows
ln -s "$(pwd)/.agents/workflows/superpowers.md" .agents/workflows/superpowers.md
```

## Verification
Start a new session and mention "superpowers". The agent should acknowledge the "Antigravity Protocol" and list available skills.
