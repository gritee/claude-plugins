# claude-plugins

A Claude Code plugin marketplace. Each plugin lives in its own repo; this repo
only holds the catalog ([.claude-plugin/marketplace.json](.claude-plugin/marketplace.json)).

## Use

```
/plugin marketplace add https://github.com/Gritee/claude-plugins.git
/plugin install session-recall@gritee
/plugin install git-contributions@gritee
```

Update later with `/plugin marketplace update gritee`.

## Plugins

| Plugin | What it does |
| --- | --- |
| [session-recall](https://github.com/Gritee/session-recall) | Turn a jam session into a recap, quiz and references, saved as JSON + Obsidian notes, with an HTML quiz runner. |
| [git-contributions](https://github.com/Gritee/identifying-your-significant-git-contributions) | Rank one author's commits in a git repository to find their most significant contributions, and optionally write them up as STAR stories. |

## Adding a plugin

1. Give the plugin repo a `.claude-plugin/plugin.json`.
2. Add an entry to `plugins` in `marketplace.json` with
   `"source": { "source": "url", "url": "https://github.com/Gritee/<repo>.git" }`.
3. Add a row to the table above.
