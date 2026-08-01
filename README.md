# Impeccable Lite

One skill. No plugin, hooks, CLI, or live mode. Just design judgment.

Impeccable Lite is a distilled, independent derivative of [Impeccable](https://github.com/pbakaus/impeccable). It keeps the frontend design guidance and removes the surrounding product ecosystem.

## Why this exists

The original Impeccable combines design guidance with commands, deterministic detectors, lifecycle hooks, live browser editing, provider adapters, subagents, installers, and release tooling.

This feature set can be useful, but it can also feel bloated when all you want is better interface decisions.

Impeccable Lite keeps the judgment layer:

- strong, coherent visual direction
- design modes for marketing, product UI, editorial work, and showcases
- practical typography, color, layout, interaction, and motion guidance
- resistance to generic AI-generated interface patterns
- accessibility, responsive behavior, performance, and edge-case requirements
- a bounded build and verification workflow

If you need deterministic design linting or live browser editing, use [full Impeccable](https://github.com/pbakaus/impeccable).

## Install

1. Choose a skills directory from the table below.
2. Create an `impeccable-lite` folder inside it.
3. Save [SKILL.md](https://raw.githubusercontent.com/ilindaniel/impeccable-lite/main/SKILL.md) in that folder.

| Platform | Project | Personal or global |
| --- | --- | --- |
| [Claude Code](https://code.claude.com/docs/en/skills) | `.claude/skills` | `~/.claude/skills` |
| [Codex](https://developers.openai.com/codex/skills) | `.agents/skills` | `~/.agents/skills` |
| [Cursor](https://cursor.com/docs/skills) | `.cursor/skills` | `~/.cursor/skills` |
| [Gemini CLI](https://geminicli.com/docs/cli/using-agent-skills/) | `.gemini/skills` | `~/.gemini/skills` |
| [GitHub Copilot](https://code.visualstudio.com/docs/agent-customization/agent-skills) | `.github/skills` | `~/.copilot/skills` |
| [Kiro](https://kiro.dev/docs/skills/) | `.kiro/skills` | `~/.kiro/skills` |
| [OpenCode](https://opencode.ai/docs/skills) | `.opencode/skills` | `~/.config/opencode/skills` |
| [Pi](https://github.com/badlogic/pi-mono/blob/main/packages/coding-agent/docs/skills.md) | `.pi/skills` | `~/.pi/agent/skills` |
| [Qoder](https://docs.qoder.com/extensions/skills) | `.qoder/skills` | `~/.qoder/skills` |
| [Rovo Dev](https://support.atlassian.com/rovo/docs/extend-rovo-dev-cli-with-agent-skills/) | `.rovodev/skills` | `~/.rovodev/skills` |
| [Mistral Vibe](https://docs.mistral.ai/vibe/code/cli/skills) | `.vibe/skills` | `~/.vibe/skills` |
| [Grok Build](https://docs.x.ai/build/features/skills-plugins-marketplaces) | `.grok/skills` | `~/.grok/skills` |
| [Antigravity IDE](https://antigravity.google/docs/skills?app=antigravity-ide) | `.agents/skills` | `~/.gemini/config/skills` |
| [Antigravity CLI](https://antigravity.google/docs/cli/gcli-migration) | `.agents/skills` | `~/.gemini/antigravity-cli/skills` |
| Trae International | `.trae/skills` | `~/.trae/skills` |
| Trae China | `.trae-cn/skills` | `~/.trae-cn/skills` |

Several platforms also recognize `.agents/skills` as a compatibility path. The table uses each platform's native directory so the installation does not depend on an alias.

### Load the skill

Start a new agent session after installation. Codex can select the skill automatically for frontend design work or be invoked explicitly with `$impeccable-lite`. Claude Code notices changes inside existing skill directories automatically, but should be restarted if the top-level skills directory was created during the session. Gemini CLI can reload with `/skills reload`, Pi with `/reload`, and Qoder requires a restart.

If an agent does not support Agent Skills, copy the contents of `SKILL.md` into its project instructions. That fallback makes the design guidance always-on instead of loading it only for relevant UI work.

## License

Apache License 2.0. Impeccable Lite contains material derived from Impeccable by Paul Bakaus, used under the same license. Modifications and original material in Impeccable Lite are copyright 2026 Daniel Ilin.
