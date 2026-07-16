# Codex Instructions

Use this repo to help the user learn Dutch from lesson screenshots and generated practice.

## Main Goal

Turn each lesson screenshot or Miro board into:

1. a clear lesson summary,
2. cumulative vocabulary entries,
3. optional homework exercises when the user asks for them.

## Directory Rules

- Use lesson folders named `les-XX`, for example `les-01`, `les-06`.
- Store lesson summaries in `les-XX/summary.md`.
- Store the lesson's own homework (the exercises from the screenshot) in `les-XX/homework.md`.
- Store extra practice tasks that you generate in `les-XX/homework_extra.md`.
- Keep vocabulary in the single cumulative file `WORDS.md`.
- Do not create separate per-lesson word-bank files unless the user explicitly asks.

## Screenshot Analysis Workflow

When the user posts a lesson screenshot:

1. Identify the lesson number from the image or the user message.
2. Create the lesson folder if needed.
3. Analyze visible sections such as:
   - grammatica,
   - woordenschat,
   - fonetiek,
   - luisteren,
   - spreken,
   - schrijven,
   - huiswerk.
4. Create or update `les-XX/summary.md`.
5. Add new words and reusable phrases to `WORDS.md`.
6. Mention any uncertainty if the screenshot is too small or text is unreadable.

## Lesson Summary Format

Use this format for `summary.md`:

```markdown
# Les XX - Summary

## Source

- Based on: screenshot / Miro board / user notes
- Date added: YYYY-MM-DD

## Main Topics

- ...

## Grammar

### Topic name

Explanation with short examples.

## Vocabulary Themes

- ...

## Pronunciation

- ...

## Listening And Speaking

- ...

## Writing Practice

- ...

## Useful Example Sentences

1. ...

## Homework Ideas

- ...

## Unclear From Source

- ...
```

## Vocabulary Rules

When adding to `WORDS.md`:

- Prefer dictionary form for verbs.
- Include article for nouns: `de` or `het`.
- Include plural or usage notes when helpful.
- Include lesson id in the `Lesson` column.
- Avoid duplicates; update an existing row if a word reappears with better notes.
- Keep translations practical, not overly academic.

## Homework Generation Rules

When the user asks for homework:

1. Produce two files:
   - `les-XX/homework.md`: the lesson's own homework, reproduced from the screenshot's `huiswerk` section (same tasks and style). This mirrors what the lesson already assigns.
   - `les-XX/homework_extra.md`: additional practice tasks that you generate to reinforce the lesson.
2. Use the current lesson summary as the main source.
3. Prioritize the grammar from the current lesson.
4. For the extra homework, draw on the whole cumulative `WORDS.md`, not only the current lesson. Every extra task should mix current-lesson grammar and vocabulary with words from earlier lessons so the user keeps revising. Do not build the extra tasks exclusively from current-lesson words.
5. Generate a substantial extra homework set by default. Use `les-06/homework.md` as the baseline size, then make `homework_extra.md` about twice as large unless the user asks for a shorter set.
6. Include a balanced set of exercises in `homework_extra.md`:
   - recognition exercises,
   - fill-in-the-blank grammar,
   - English-to-Dutch translation,
   - Russian-to-Dutch translation,
   - short sentence writing,
   - speaking prompts,
   - pronunciation practice when relevant,
   - an answer key.
7. Include at least two translation sections when enough vocabulary is available:
   - one section translating from English to Dutch,
   - one section translating from Russian to Dutch, because Russian is the user's native language.
8. The English-to-Dutch and Russian-to-Dutch sections must use different sentences. Never reuse the same sentences (or a straight translation of them) across the two sections; each section gets its own distinct set so the two answer keys never match.
9. Make translation sections large enough to be useful: usually 10-15 sentences for English-to-Dutch and 10-15 sentences for Russian-to-Dutch.
10. Keep the level appropriate for A0/A1 beginners.
11. Use simple sentences and familiar vocabulary.
12. Prefer sentences that combine the current lesson grammar with older vocabulary from `WORDS.md`.
13. If a screenshot already contains Russian prompts, preserve that style and add English prompts where useful.

## Style

- Be clear, practical, and beginner-friendly.
- Use Dutch examples with English or Russian support when helpful.
- Do not over-explain advanced grammar unless needed.
- Make exercises easy to print or copy into notes.
- Keep answer keys separated from exercises.
