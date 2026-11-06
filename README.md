# claude-plugins

A Claude Code plugin marketplace. Each plugin lives in its own repo; this repo
only holds the catalog ([.claude-plugin/marketplace.json](.claude-plugin/marketplace.json)).

## Use

```
/plugin marketplace add Gritee/claude-plugins
/plugin install session-recall@gritee
```

Update later with `/plugin marketplace update gritee`.

## Plugins

| Plugin | What it does |
| --- | --- |
| [session-recall](https://github.com/Gritee/session-recall) | Turn a jam session into a recap, quiz and references, saved as JSON + Obsidian notes, with an HTML quiz runner. |

## Adding a plugin

1. Give the plugin repo a `.claude-plugin/plugin.json`.
2. Add an entry to `plugins` in `marketplace.json` with
   `"source": { "source": "github", "repo": "Gritee/<repo>" }`.
3. Add a row to the table above.
