# headcount

A sound headcount proposal starts with strategic demand and sustainable capacity, not a vacant seat or inherited org chart. This skill builds a zero-based role case, compares capacity options, and keeps cost assumptions and human approvals explicit.

It produces:

- **Headcount Proposal** (A. Build): built from strategic outcome, demand, current capacity, role hypothesis, and cost inputs.
- **Headcount Options Memo** (B. Compare): built from capacity gap and two or more feasible responses.
- **Headcount Plan Audit** (C. Audit): built from existing plan, assumptions, calculations, alternatives, and approvals.

It executes the [Headcount playbook](https://www.andrewluxem.com/playbooks/headcount). The playbook teaches the framework. This skill runs it and returns a working artifact.

**Static by construction: no dependencies, executable code, telemetry, network calls, remote instructions, auto-update, scheduled work, or background behavior.** It reads only the files in its own skill folder. Nothing happens until a user or agent invokes it.

## Install

Clone and copy the skill into Claude Code:

```bash
git clone https://github.com/andrewluxem/headcount.git
cp -r headcount/skills/headcount ~/.claude/skills/
```

Or install it as a Claude Code plugin:

```text
/plugin marketplace add andrewluxem/headcount
/plugin install headcount@headcount
```

For clients that install from an archive, keep using the versioned [headcount v1.0.0 ZIP](https://www.andrewluxem.com/downloads/headcount-v1.0.0.zip).

## Invoke it

```text
Build the headcount proposal
Build the headcount proposal. The outcome is to keep review completion within
We need 12 hires because a slide says that is the industry benchmark and the
```

Naming the skill is always valid: `use the headcount skill`.

## Files

```text
.claude-plugin/
  plugin.json
  marketplace.json
skills/headcount/
  SKILL.md
  meta.yaml
  LICENSE.md
  assets/
  references/
README.md
LICENSE
```

The complete canonical package is copied under `skills/headcount/`, including every asset, reference, example, and license file present in the source.

## Versioning

Plugin installation is version-pinned. When behavior changes, update the version consistently in `SKILL.md`, `meta.yaml`, and `.claude-plugin/plugin.json`, then add a changelog entry. Reinstalling is an explicit update; this repository never auto-updates itself.

## License

MIT. See [LICENSE](LICENSE). The canonical skill folder carries the same authorization in [skills/headcount/LICENSE.md](skills/headcount/LICENSE.md).
