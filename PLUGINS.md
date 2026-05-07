# Plugins

> **Note** — This is a fork of [`Leonxlnx/taste-skill`](https://github.com/Leonxlnx/taste-skill) that adds Claude Code and Codex CLI plugin manifests. The install URLs below point to this fork (`seungyeop-lee/taste-skill`); the upstream `npx skills add` URL in [`README.md`](README.md) is unchanged.

This guide covers installing the skills as a plugin in **Claude Code** and **OpenAI Codex CLI**. For the original `npx skills add` flow and manual copy-paste, see [`README.md`](README.md#installing).

## Claude Code

Inside Claude Code, register this repository as a marketplace and install the plugin:

```
/plugin marketplace add seungyeop-lee/taste-skill
/plugin install taste-skill@taste-skill
```

After installation, all skills under `skills/` become available, namespaced as `taste-skill:<skill-name>` (for example, `taste-skill:design-taste-frontend`).

## Codex CLI

Register the marketplace from your terminal:

```
codex plugin marketplace add seungyeop-lee/taste-skill
```

Then open Codex CLI, browse to the plugin entry for `taste-skill`, and select **Install plugin**. The official install flow is interactive — there is no `codex plugin install <name>` terminal subcommand.

Once installed, Codex auto-discovers the skills under `skills/` (each subdirectory with a `SKILL.md` registers as a skill). Start a new thread and ask Codex to use the plugin or a specific skill. To refresh later, run `codex plugin marketplace upgrade taste-skill`.

## Skill install names

The skills bundled in this plugin (install names from each `SKILL.md` frontmatter):

- `design-taste-frontend`
- `gpt-taste`
- `image-to-code`
- `redesign-existing-projects`
- `high-end-visual-design`
- `full-output-enforcement`
- `minimalist-ui`
- `industrial-brutalist-ui`
- `stitch-design-taste`
- `imagegen-frontend-web`
- `imagegen-frontend-mobile`
- `brandkit`

For what each skill does, see the [Skills section in `README.md`](README.md#skills).

## Other install methods

For `npx skills add` and manual copy-paste, see [`README.md` § Installing](README.md#installing).
