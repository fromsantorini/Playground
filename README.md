# Playground for Codex

Creates interactive HTML playgrounds: self-contained single-file explorers that let users configure something visually through controls, see a live preview, and copy out a prompt.

This repository is a Codex-compatible adaptation of Anthropic's `playground` Claude plugin.

## Origin

- Original project: `claude-plugins-official/plugins/playground`
- Original author: Anthropic
- License: Apache License 2.0

This adaptation keeps the original Apache License 2.0 license text and adds Codex-specific plugin metadata.

## Changes In This Adaptation

- Added `.codex-plugin/plugin.json` for Codex plugin discovery.
- Updated Claude-specific wording in the skill and README to refer to Codex.
- Changed browser-launch guidance to Codex-friendly delivery guidance.
- Kept the original skill templates and Apache License 2.0 license text.

## Not Official

This project is an independent Codex-compatible adaptation. It is not affiliated with, sponsored by, or endorsed by Anthropic.

Anthropic names and references are used only to identify the origin of the Apache-2.0-licensed upstream work.

## What Is A Playground?

A playground is a self-contained HTML file with:

- Interactive controls on one side
- A live preview on the other
- A prompt output at the bottom with a copy button

The user adjusts controls, explores visually, then copies the generated prompt back into Codex.

## When To Use

Use this plugin when the user asks for an interactive playground, explorer, or visual tool for a topic, especially when the input space is large, visual, or structural and hard to express as plain text.

## Templates

The skill includes templates for common playground types:

- `design-playground`: visual design decisions such as components, layouts, spacing, color, and typography
- `data-explorer`: data and query building such as SQL, APIs, pipelines, and regex
- `concept-map`: learning and exploration such as concept maps, knowledge gaps, and scope mapping
- `document-critique`: document review with suggestions and approve/reject/comment workflow
- `diff-review`: code review for diffs, commits, and PRs
- `code-map`: codebase architecture, component relationships, data flow, and layer diagrams

## Installation

Add this plugin to a Codex plugin marketplace to enable the playground skill.

For a marketplace repository, use this structure:

```text
repo-root/
  marketplace.json
  plugins/
    playground/
      .codex-plugin/plugin.json
      skills/
      README.md
      LICENSE
      NOTICE
```

The marketplace entry should point to `./plugins/playground`.

## License

This adaptation is distributed under the Apache License 2.0, the same license as the upstream work. See `LICENSE` and `NOTICE`.
