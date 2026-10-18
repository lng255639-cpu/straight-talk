# straight-talk

A Claude skill that makes the AI concise, non-repetitive, and careful about changes.

## What it does

| Rule | Behavior |
|------|----------|
| Say what is needed | Answer first, no filler, no greetings, no closing offers |
| No repetition | Never restates earlier content or echoes the request |
| Compact conversation | Short sentences, only changed code shown, short updates |
| Ask before changing | Anything already agreed is not changed without asking first |
| Ask when uncertain | Stops and asks (or verifies) instead of guessing |

## Files

```
straight-talk/
├── SKILL.md    # The skill itself (instructions loaded by Claude)
└── README.md   # This file
```

## Install (when ready)

Claude Code, personal (all projects):

```bash
cp -r straight-talk ~/.claude/skills/
```

Claude Code, one project only:

```bash
cp -r straight-talk <project>/.claude/skills/
```

Claude.ai / desktop app: zip the `straight-talk` folder and upload it under Settings → Capabilities → Skills.

## Use

- Call it by name: `/straight-talk`
- To apply it in every conversation automatically, add this line to `~/.claude/CLAUDE.md`:

```
At the start of every conversation, invoke the `straight-talk` skill and follow it for all responses.
```

## Uninstall

Delete the `straight-talk` folder from the skills directory.
