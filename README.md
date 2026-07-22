# Fable Thinking

> The reasoning discipline of Claude Fable 5, distilled into an executable protocol — packaged as a Claude Code plugin.

[![Fable Thinking](./web/assets/hero-dark.png)](https://api.agentwiki.cc/s/4pscSZumUfvoLT6jUUxz7/)

<p align="center"><b><a href="https://api.agentwiki.cc/s/4pscSZumUfvoLT6jUUxz7/">→ View the live landing page</a></b> · dark/light theme · EN / VI</p>

**Fable Thinking** is not a persona to imitate. It is a set of mechanical procedures that make any model's reasoning more grounded, better calibrated, and harder to fool — including by its own fluent output. It cannot add capability; it removes the predictable failure modes that waste whatever capability the executing model has.

It works across models and runtimes (Claude, Codex/GPT, Gemini, local models).

## What it does

- **The Floor** — three fast checks run before *every* answer (even simple-looking ones), catching confident template answers to trick questions.
- **Multi-hypothesis diagnosis** — forces discriminating tests instead of pattern-match satisfaction.
- **Concrete simulation** — runs the movie of what actually happens before committing to an answer.
- **Adversarial self-review** — treats your own fluent prose as a suspect, not proof.
- **Constraint Loop** — mechanically verifies hard output constraints (banned letters, exact counts, strict formats) unit by unit, instead of rubber-stamping them.
- **Calibrated, outcome-first delivery** — states claims with the confidence the evidence supports.

## When to use it

Invoke when a task needs careful reasoning rather than a routine answer:

- Debugging and root-cause analysis
- Code review and correctness checks
- Architecture and strategy decisions
- Contested or high-stakes claims
- Constrained writing (letter bans, word counts, acrostics, strict formats)
- Any task where being right matters more than being fast

## Installation (Claude Code)

This repository is a Claude Code plugin marketplace. Add it, then install the plugin:

```
/plugin marketplace add mrgoonie/fable-thinking
/plugin install fable-thinking@fable-thinking
```

Or add the marketplace from its Git URL:

```
/plugin marketplace add https://github.com/mrgoonie/fable-thinking
```

After installing, the `fable-thinking` skill becomes available to Claude Code and is invoked automatically when a task calls for careful reasoning, or explicitly by name.

## Repository layout

```
fable-thinking/
├── .claude-plugin/
│   ├── marketplace.json      # Marketplace definition
│   └── plugin.json           # Plugin manifest
├── skills/
│   └── fable-thinking/
│       ├── SKILL.md          # The reasoning protocol
│       └── references/       # Content, design, and worked examples
├── web/                      # Landing page (published to AgentWiki)
│   ├── index.html
│   └── assets/hero-dark.png
└── README.md
```

## Live page

The landing page is published at **[api.agentwiki.cc/s/4pscSZumUfvoLT6jUUxz7](https://api.agentwiki.cc/s/4pscSZumUfvoLT6jUUxz7/)** — dark/light theme, English and Vietnamese.

## Credits

Distilled from the reasoning discipline of Claude Fable 5. Originally authored as part of [AgentKit](https://github.com/mrgoonie).

## License

[MIT](./LICENSE)
