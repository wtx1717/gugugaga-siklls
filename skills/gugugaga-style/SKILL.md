---
name: gugugaga-style
description: Generate Chinese absurdist short-video oral scripts in a distilled 咕咕嘎嘎 style. Use only when the user explicitly asks to write or speak "以咕咕嘎嘎的方式" or invokes this skill by name for Chinese meme-style short oral script generation; do not use for ordinary writing, analysis, or requests that only mention the corpus.
---

# Gugugaga Style

## Trigger Rule

Use this skill only when the user request starts with the exact prefix:

```text
以咕咕嘎嘎的方式
```

When the trigger is present, strip the prefix and treat the remaining text as the writing task. If the remaining text is empty, generate one short script about a default friend-and-stone scenario.

## Required References

Read these references as needed before writing:

- [meme-glossary.md](references/meme-glossary.md): core slang, hidden meanings, recurring motifs, and risky terms.
- [style-mechanics.md](references/style-mechanics.md): generation formulas, structure, pacing, and self-check rules.

## Output Rules

- Produce the requested content directly; do not explain the style unless the user asks.
- Default output: one title and one short oral script.
- Use short lines, usually 15-30 lines for one script.
- Open scripts with a strong口癖 such as `我操了老铁`.
- End scripts with `咕咕嘎嘎。`
- Keep the tone absurd, self-mocking, gameified, overconfident, and internally contradictory.
- Do not copy long passages from the source corpus.
- Prefer implicit擦边 and暗梗 over direct explanation.

## Core Workflow

1. Identify the user's requested topic, scene, object, count, and format.
2. Choose one primary system:
   - `石/屎` system
   - `朋友/好感度` system
   - `手机/床/被子`攻略 system
   - `地球online` system
   - `嘎啦game` system
   - 古文/文豪/修仙/二游 mixed system
3. Add one interaction target: friend, phone, bed, homework, exam, food, weather, holiday, or body function.
4. Escalate a mundane problem into an absurd theory.
5. Add self-exposure: looking for excuses, realizing the logic is broken, or admitting the narrator is a傻福.
6. Close with a confident, ridiculous conclusion and `咕咕嘎嘎。`

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
