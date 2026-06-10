# Output Modes

Choose the smallest mode that satisfies the user.

## Default: Title + Short Script

Use when the user says `以咕咕嘎嘎的方式说/写...` without extra format requirements.

Output:

```text
[one title]

[15-30 short oral-script lines]
咕咕嘎嘎。
```

## Titles Only

Use when the user asks for标题,选题,标题库, or multiple hooks.

Rules:

- Return a numbered list unless the user requests another format.
- Keep each title one punchline long.
- Use one clear system per title.
- Do not add explanations unless requested.

## Multi-Script Batch

Use when the user asks for several scripts.

Rules:

- Give each script a title.
- Vary the primary system across scripts.
- Keep each script shorter than the default if many are requested.
- Avoid repeating the same opener every time; `我操了老铁` can appear in one or two, not all.

## Rewrite Mode

Use when the user supplies draft text and asks to改成咕咕嘎嘎风格.

Workflow:

1. Preserve the user's topic and intended punchline.
2. Replace plain explanation with one system lens.
3. Add口播 rhythm, self-exposure, and a compact ending.
4. Do not preserve wording if it fights the style.

## Analysis Mode

Use when the user asks why a line works, how to沉淀, or how to拆梗.

Output sections can be:

- `梗词 / 隐梗`
- `语义映射`
- `笑点机制`
- `可迁移句式`
- `避免事项`

Keep analysis concise. Do not include full raw corpus passages.

## Documentation Mode

Use when the user asks to update the skill,整理文档,扩充词库, or add reference rules.

Rules:

- Prefer distilled rules over source transcripts.
- Put detailed content in `references/`, not `SKILL.md`.
- Keep `SKILL.md` as navigation plus core workflow.
- Preserve the existing eight-file reference architecture unless the user changes it.
