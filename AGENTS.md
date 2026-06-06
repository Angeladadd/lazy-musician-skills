# AGENTS.md

When working on this repository, follow these conventions:

## Skill structure
- Skills live under `.opencode/skills/<skill-name>/SKILL.md`
- Each SKILL.md must have YAML frontmatter with: `name`, `description`, `license`, `compatibility: opencode`, and `metadata` (domain + instrument)
- Keep descriptions concise — one sentence in the frontmatter
- Use clear numbered phases or workflow steps in the body

## Naming
- Skill directory names use kebab-case (e.g., `chords-arrangement-from-melody`)
- Description metadata should use `music-theory` as the domain
- Instrument metadata should describe the primary instrument (use `any` if instrument-agnostic)

## Commits
- Use conventional commit style: `Add <skill-name> skill for <short description>`
- Always stage new skills with `git add .opencode/skills/<skill-name>/`

## Checking
- This repo uses no linters or tests — just verify the YAML frontmatter is valid and the skill renders correctly as markdown.
