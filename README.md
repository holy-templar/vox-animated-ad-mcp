# Vox-Style Animated Ad Skill — MaxFusion MCP Edition (v1.5)

An agent skill that turns one sentence into a complete Vox-style paper-collage animated video — script, per-clip prompts, image and video generation, clip chaining — all from a single chat session. The agent is the creative director; the [MaxFusion AI MCP](https://maxfusion.ai?via=UGC-IG) is the engine that generates every image and clip (Google Omni, 10-second clips).

Two content modes, chosen at intake:

- **AD** — a product/offer ad written in 9-figure direct-response style.
- **PURE EXPLAINER** — editorial storytelling that sells nothing (faceless-channel ready).

The consistency trick: with chaining ON, the skill extracts the last frame of each finished clip and passes it as a reference into the next clip's generation call — which is why the result looks like one continuous animation instead of disconnected AI shots.

## Requirements

- An agent that can load this file as a skill or system context (built for Claude; works with any agent that can follow it).
- The **MaxFusion AI MCP** connected to your agent — this is the generation engine; the skill drives it entirely from chat, never through a canvas or UI. Get access at [maxfusion.ai](https://maxfusion.ai?via=UGC-IG).

Note for agents: video generation is a paid action. Confirm with your human before submitting generation jobs.

## Install (Claude Code)

```
your-project/
└── .claude/
    └── skills/
        └── vox-animated-ad-mcp/
            └── SKILL.md   ← this file
```

Then trigger with: "make/run the Vox ad", "vox mcp", "vox explainer", or any Vox-style / paper-collage / explainer request.

Other agents: give your agent the raw `SKILL.md` as context and tell it to follow the skill.

## License

[GNU AGPL v3.0](LICENSE) — Copyright (C) 2026 Maxfusion AI.

Free to use, study, modify and share. If you modify it and let others use it —
including over a network — the modified version must be released under the
same license.
