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
4. Include a balanced set of exercises:
   - recognition exercises,
   - fill-in-the-blank grammar,
   - translation into Dutch,
   - short sentence writing,
   - speaking prompts,
   - pronunciation practice when relevant,
   - an answer key.
5. Keep the level appropriate for A0/A1 beginners.
6. Use simple sentences and familiar vocabulary.
7. If using Russian prompts from the screenshot, also allow English prompts when useful.
8. Put generated homework in `les-XX/homework.md`.

## Style

- Be clear, practical, and beginner-friendly.
- Use Dutch examples with English or Russian support when helpful.
- Do not over-explain advanced grammar unless needed.
- Make exercises easy to print or copy into notes.
- Keep answer keys separated from exercises.
