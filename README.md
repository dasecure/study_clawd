# 📚 Study Clawd

System prompts and workspace files for building AI agents like [Clawdbot](https://github.com/clawdbot/clawdbot).

## Files

| File | Purpose |
|------|---------|
| `AGENTS.md` | Agent behavior, memory management, workspace rules |
| `SOUL.md` | Personality, tone, core values |
| `USER.md` | Info about the human you're helping |

## How It Works

These files are loaded into the AI's context at the start of each session:

```
┌─────────────────────────────────────────┐
│           SYSTEM PROMPT                 │
│  ┌─────────────────────────────────┐    │
│  │  AGENTS.md (how to behave)      │    │
│  │  SOUL.md (who you are)          │    │
│  │  USER.md (who you're helping)   │    │
│  │  memory/*.md (recent context)   │    │
│  └─────────────────────────────────┘    │
└─────────────────────────────────────────┘
              ↓
        AI has persistent
        "memory" and personality
```

## Usage

1. Fork this repo
2. Edit the files to match your preferences
3. Point your AI agent to load these files into its system prompt

## See Also

- [Clawdbot](https://github.com/clawdbot/clawdbot) — The full AI agent framework
- [MiniBot](/home/clawd/clawd/minibot) — A minimal ~200 line implementation

## License

MIT
