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
- Store generated homework in `les-XX/homework.md`.
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

1. Use the current lesson summary as the main source.
2. Use `WORDS.md` to reuse words from previous lessons.
3. Prioritize the grammar from the current lesson.
4. Generate a substantial homework set by default. Use `les-06/homework.md` as the baseline size, then make new homework about twice as large unless the user asks for a shorter set.
5. Include a balanced set of exercises:
   - recognition exercises,
   - fill-in-the-blank grammar,
   - English-to-Dutch translation,
   - Russian-to-Dutch translation,
   - short sentence writing,
   - speaking prompts,
   - pronunciation practice when relevant,
   - an answer key.
6. Include at least two translation sections when enough vocabulary is available:
   - one section translating from English to Dutch,
   - one section translating from Russian to Dutch, because Russian is the user's native language.
7. Make translation sections large enough to be useful: usually 10-15 sentences for English-to-Dutch and 10-15 sentences for Russian-to-Dutch.
8. Keep the level appropriate for A0/A1 beginners.
9. Use simple sentences and familiar vocabulary.
10. Prefer sentences that combine the current lesson grammar with older vocabulary from `WORDS.md`.
11. If a screenshot already contains Russian prompts, preserve that style and add English prompts where useful.
12. Put generated homework in `les-XX/homework.md`.

## Style

- Be clear, practical, and beginner-friendly.
- Use Dutch examples with English or Russian support when helpful.
- Do not over-explain advanced grammar unless needed.
- Make exercises easy to print or copy into notes.
- Keep answer keys separated from exercises.
