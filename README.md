# Yash Verma's Claude Code plugins

A [Claude Code](https://claude.com/claude-code) plugin marketplace. Add it once, then install any plugin listed here.

## Add the marketplace

In Claude Code:

```
/plugin marketplace add yashverma2110/claude-plugins
```

Then browse with `/plugin`, or install a plugin directly as shown below. To get new plugins and versions later:

```
/plugin marketplace update yashverma
```

## Plugins

| Plugin | What it does | Install |
|---|---|---|
| [maxlearn](https://github.com/yashverma2110/maxlearn) | A study companion beside your chat: teaches the ideas behind your daily work in short lessons, turns them into flashcards, and schedules reviews with FSRS or SM-2 spaced repetition | `/plugin install maxlearn@yashverma` |

Plugins run with the same access as Claude Code. Each plugin's README says what it uses and how to turn it off.

## Add a plugin to this marketplace

Each plugin lives in its own repository. List it in `.claude-plugin/marketplace.json`:

```json
{
  "name": "my-plugin",
  "source": { "source": "github", "repo": "yashverma2110/my-plugin" },
  "description": "One line on what it does"
}
```

Check it with `claude plugin validate . --strict`.

## License

[MIT](LICENSE)
