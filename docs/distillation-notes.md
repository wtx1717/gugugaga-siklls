# Distillation Notes

This document describes the public, high-level distillation process. It intentionally avoids publishing the full source corpus, raw subtitles, and training annotations.

## Goal

Extract reusable writing mechanics from a short-video corpus and convert them into a compact Codex skill.

The final skill should help a model generate new scripts with similar structure, pacing, and motif logic without copying long source passages.

## Process

1. Collect source videos locally.
2. Extract burned-in subtitles with OCR.
3. Correct obvious OCR errors.
4. Group recurring motifs:
   - stone/shit euphemism
   - friend as victim/rival/攻略 target
   - galgame logic for daily life
   - reality as 地球online
   - phone, sleep, food, homework, exams, holidays
   - classical text, cultivation, ACG, and game crossover jokes
5. Convert motifs into:
   - `meme-glossary.md`
   - `semantic-map.md`
   - `style-mechanics.md`
   - `tone-and-rhythm.md`
   - `structures.md`
   - `examples.md`
   - `output-modes.md`
   - `avoid.md`
   - concise rules inside `SKILL.md`
6. Keep raw materials out of the public repository.

## Public vs Private Split

Public files:

- distilled rules
- glossary
- generation mechanics
- install instructions
- small examples

Private files:

- source videos
- raw subtitle dumps
- full training notes
- large intermediate OCR outputs

## Quality Checks

Before publishing a new version:

- Confirm all public Markdown files are UTF-8 and readable.
- Confirm `SKILL.md` has only `name` and `description` in YAML frontmatter.
- Confirm trigger wording in README and `SKILL.md` matches.
- Confirm `SKILL.md` links all eight reference files.
- Confirm examples are newly generated and not copied from the source corpus.
- Confirm ignored local materials are not staged for commit.
