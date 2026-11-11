# automation-templates

One markdown file per automation. Each file is a complete, self-contained recipe for an agent bot (e.g. a Grok Bot, or any agent with a shell plus the listed connectors). It covers what the bot does, what it needs, the questions it asks you, the step-by-step procedure, gotchas, a ready-to-schedule routine prompt, and safety rules.

## Use a template

1. Pick a file (e.g. `product-showcase.md`).
2. Create a new bot and paste the whole file in as its instructions, or attach it and say "set this up".
3. Connect what the **Prerequisites** section lists (CLI logins, GitHub, Slack, …).
4. Answer the bot's **setup questions** once; it saves them and creates the schedule.
5. It posts on its own from the first run. Ask for draft mode during setup if you want to approve posts first.

## Templates

| File | What it does |
|---|---|
| `product-showcase.md` | Watches PRs merged to staging, records the visible change with Revyl, posts a redacted clip + PR link to Slack. |

## Contributing

Keep it to one `.md`. No private ids, hostnames, emails or names: use `<PLACEHOLDERS>`. Keep the file short, with small inline snippets instead of helper scripts.
