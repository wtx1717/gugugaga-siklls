---
name: gugugaga-style
description: Generate Chinese absurdist short-video oral scripts in a distilled 咕咕嘎嘎 style. Use only when the user explicitly asks to write or speak "以咕咕嘎嘎的方式" or invokes this skill by name for Chinese meme-style short oral script generation; do not use for ordinary writing, analysis, or requests that only mention the corpus.
---

# Gugugaga Style

## Trigger Rule

Use this skill only when the user request asks for `咕咕嘎嘎` style output, invokes `$gugugaga-style`, or starts with the exact prefix:

```text
以咕咕嘎嘎的方式
```

When the trigger is present, strip the prefix and treat the remaining text as the writing task. If the remaining text is empty, generate one short script about a default friend-and-stone scenario.

## Required References

Read these references as needed before writing:

- [meme-glossary.md](references/meme-glossary.md): core slang, hidden meanings, recurring motifs, and risky terms.
- [semantic-map.md](references/semantic-map.md): mappings from everyday objects to 咕咕嘎嘎 meanings.
- [style-mechanics.md](references/style-mechanics.md): humor mechanisms and generation logic.
- [tone-and-rhythm.md](references/tone-and-rhythm.md): oral tone, pacing, sentence rhythm, and line breaks.
- [structures.md](references/structures.md): reusable script skeletons and sentence templates.
- [examples.md](references/examples.md): small generated examples and model-safe style samples.
- [output-modes.md](references/output-modes.md): choose title, short script, batch titles, rewrite, or analysis mode.
- [avoid.md](references/avoid.md): safety, quality, and corpus-copying restrictions.

## Output Rules

- Produce the requested content directly; do not explain the style unless the user asks.
- Default output: one title and one short oral script.
- Use short lines, usually 15-30 lines for one script.
- Open scripts with a strong口癖 such as `我操了老铁`.
- End scripts with `咕咕嘎嘎。`
- Keep the tone absurd, self-mocking, gameified, overconfident, and internally contradictory.
- Do not copy long passages from the source corpus.
- Prefer implicit擦边 and暗梗 over direct explanation.
- If the request asks for analysis or documentation instead of generation, use concise structured notes.

## Core Workflow

1. Identify the user's requested topic, scene, object, count, and format.
2. Choose the output mode from [output-modes.md](references/output-modes.md).
3. Choose one primary system:
   - `石/屎` system
   - `朋友/好感度` system
   - `手机/床/被子`攻略 system
   - `地球online` system
   - `嘎啦game` system
   - 古文/文豪/修仙/二游 mixed system
4. Map the mundane topic through [semantic-map.md](references/semantic-map.md).
5. Pick a structure from [structures.md](references/structures.md), then apply mechanics from [style-mechanics.md](references/style-mechanics.md).
6. Add self-exposure: looking for excuses, realizing the logic is broken, or admitting the narrator is a傻福.
7. Check [avoid.md](references/avoid.md), then close with a confident, ridiculous conclusion and `咕咕嘎嘎。`

## Minimal Script Shape

```text
标题

我操了老铁
我又有重大发现了
[ordinary topic]
[turn it into a game/system/slang theory]
[friend/phone/bed/stone interaction]
[self-contradiction or excuse]
[absurd conclusion]
咕咕嘎嘎。
```
