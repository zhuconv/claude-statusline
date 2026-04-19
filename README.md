# claude-statusline

> Fork of [kamranahmedse/claude-statusline](https://github.com/kamranahmedse/claude-statusline) with:
> - Live effort level detection (reads from transcript JSONL, supports `max` / `xhigh`)
> - Weekly usage on the first line (5-hour bar and extra-credits line removed)
> - Compact single-line layout

Configure your Claude Code statusline to show limits, directory and git info

![demo](./.github/demo.png)

## Install

Run the command below to set it up

```bash
npx github:zhuconv/claude-statusline
```

It backups your old status line if any and copies the status line script to `~/.claude/statusline.sh` and configures your Claude Code settings.

## Requirements

- [jq](https://jqlang.github.io/jq/) — for parsing JSON
- curl — for fetching rate limit data
- git — for branch info

On macOS:

```bash
brew install jq
```

## Uninstall

```bash
npx github:zhuconv/claude-statusline --uninstall
```

If you had a previous statusline, it restores it from the backup. Otherwise it removes the script and cleans up your settings.

## Updating

`npx github:` caches clones, so to pull the latest version:

```bash
npx --yes github:zhuconv/claude-statusline
```

Or pin to a tag:

```bash
npx github:zhuconv/claude-statusline#v1.0.0
```

## License

MIT
