# Installing Superpowers for Antigravity

Follow these steps to enable Superpowers skills in your Antigravity environment.

## 1. Clone the repository

```bash
git clone https://github.com/obra/superpowers.git ~/skills/superpowers
```

## 2. Register skills

Choose one of the following methods to register the skills.

### Option A: Global Installation (All Projects)
Create a symlink in the Antigravity global skills directory:

```bash
mkdir -p ~/.gemini/antigravity/skills
ln -s ~/skills/superpowers/skills ~/.gemini/antigravity/skills/superpowers
```

### Option B: Workspace-specific Installation (Current Project Only)
Create a symlink in your project's local agent directory:

```bash
mkdir -p .agent/skills
ln -s ~/skills/superpowers/skills .agent/skills/superpowers
```

## 3. Verify

Start a new session and mention "superpowers". The agent should acknowledge the discovery of Superpowers skills.
