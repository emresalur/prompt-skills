# Prompt Engineering Skills for Claude Code

Two skills that help you improve your prompting through real-time feedback and session-level analysis.

## Skills

### `/prompt-review`
Analyzes your most recent prompt for clarity, ambiguity, missing context, and scope issues. Returns a score, diagnosis, and a rewritten version.

### `/session-review`
Reviews your entire conversation at the end of a session. Scores your overall communication, highlights what worked, what didn't, and identifies recurring patterns across sessions.

## Installation

Copy the skill folders into your Claude Code skills directory:

**Per-project** (available in one repo):
```bash
cp -r prompt-review session-review /path/to/your/project/.claude/skills/
```

**Global** (available across all projects):
```bash
cp -r prompt-review session-review ~/.claude/skills/
```

## Usage

In any Claude Code conversation:

```
/prompt-review    # after writing a prompt you want feedback on
/session-review   # at the end of a session
```

## Tips

- Run `/prompt-review` on prompts that got unexpected results to understand why
- Run `/session-review` at the end of each working session to build awareness of your habits
- The session-review skill tracks recurring patterns if you keep a log — add a memory file to persist feedback across conversations
