# agent-skills

Public [Agent Skills](https://agentskills.io) for JonesLabs products. Each skill teaches an AI coding agent how to use one product's public API: how to get an API key, how to authenticate, which endpoints exist, and how to handle limits and errors.

The skills follow the [Agent Skills specification](https://agentskills.io/specification). They work with any agent that supports skills, such as Claude Code, Cursor, Codex and GitHub Copilot.

## Skills

| Skill | Product | What it covers |
|-------|---------|----------------|
| [`accesshawk`](skills/accesshawk/SKILL.md) | [AccessHawk](https://accesshawk.ai) | Run WCAG accessibility scans with the hosted REST API: create projects, start scans, poll for results, verify webhooks. Needs an API key on a Hobby, Pro or Team plan. |
| [`serenereader`](skills/serenereader/SKILL.md) | [SereneReader](https://serenereader.com) | Read your RSS feeds and articles with the read-only REST API: list feeds, filter and page through articles, check usage. Needs an API key on a Pro or Team plan. |

## Install

Install one skill with the [`skills`](https://skills.sh) CLI:

```bash
npx skills add joneslabs-llc/agent-skills --skill accesshawk
npx skills add joneslabs-llc/agent-skills --skill serenereader
```

Run `npx skills add joneslabs-llc/agent-skills` to pick from the list.

## Related

AccessHawk's scan engine is open source as [a11yhawk](https://github.com/charlesjones-dev/a11yhawk). To run accessibility scans locally, without an AccessHawk account, install its skill:

```bash
npx skills add charlesjones-dev/a11yhawk
```

## License

[MIT](LICENSE)
