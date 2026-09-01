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
7. Write all explanatory content in Russian. Keep Dutch forms, examples, dialogues, and source texts in Dutch. English may appear only as source text in exercises that explicitly ask the learner to translate from English into Dutch.

## Lesson Summary Format

Use this format for `summary.md`:

```markdown
# Урок XX — конспект

## Источник

- Материал: скриншот / доска Miro / заметки пользователя
- Дата добавления: YYYY-MM-DD

## Основные темы

- ...

## Грамматика

Объясняйте каждую грамматическую тему по-русски. Нидерландские формы и примеры оставляйте на нидерландском.

### Название темы

Объяснение с короткими примерами.

## Темы лексики

- ...

## Произношение

- ...

## Аудирование и устная речь

- ...

## Письменная практика

- ...

## Полезные примеры

1. ...

## Идеи для домашней работы

- ...

## Неясности в источнике

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
3. Write every task heading, actionable instruction, purpose statement, label, note, and example explanation in Russian. Keep Dutch forms, answer options, dialogues, and other Dutch study material in Dutch. In an English-to-Dutch translation exercise, keep the English source sentences in English, but write the heading and instructions in Russian. Do not add English explanations elsewhere.
4. Prioritize the grammar from the current lesson.
5. For the extra homework, draw on the whole cumulative `WORDS.md`, not only the current lesson. Every extra task should mix current-lesson grammar and vocabulary with words from earlier lessons so the user keeps revising. Do not build the extra tasks exclusively from current-lesson words.
6. Generate a substantial extra homework set by default. Use `les-06/homework.md` as the baseline size, then make `homework_extra.md` about twice as large unless the user asks for a shorter set.
7. Always use the same set of task types as `les-10/homework_extra2.md`, in this order:
   - fill-in-the-blank grammar for the current lesson's main grammar,
   - choose and fill in the comparative or superlative form (`comparatief` / `superlatief`),
   - `de`-woord or `het`-woord recognition,
   - Russian-to-Dutch translation,
   - English-to-Dutch translation,
   - ontkennende zinnen (`niet` / `geen`),
   - vragen (yes/no questions plus questions with a question word),
   - an answer key for every section.
   Add or adapt a grammar fill-in section to match the current lesson's grammar, but keep the overall structure above.
   Never generate tasks that cannot have a fixed answer key (e.g. `Spreken`, `Vertellen`, free writing / describe-a-picture prompts). Every task must have answers in the answer key.
8. Include at least two translation sections when enough vocabulary is available:
   - one section translating from English to Dutch,
   - one section translating from Russian to Dutch, because Russian is the user's native language.
9. The English-to-Dutch and Russian-to-Dutch sections must use different sentences. Never reuse the same sentences (or a straight translation of them) across the two sections; each section gets its own distinct set so the two answer keys never match.
10. Make translation sections large enough to be useful: usually 10-15 sentences for English-to-Dutch and 10-15 sentences for Russian-to-Dutch.
11. Keep the level appropriate for A0/A1 beginners.
12. Use simple sentences and familiar vocabulary.
13. Prefer sentences that combine the current lesson grammar with older vocabulary from `WORDS.md`.
14. If a screenshot already contains Russian prompts, preserve that style. Do not add English prompts except as source sentences in a dedicated English-to-Dutch translation exercise.

### User's Standard Homework Requirements

Apply these requirements to generated extra homework unless the user explicitly asks for a different format:

1. Include exercises covering:
   - comparative and superlative forms, with context determining which form is required,
   - direct, indirect, and possessive pronouns,
   - negative sentences,
   - questions,
   - large numbers written in words, including ordinal numbers,
   - sentence building with conjunctions learned so far,
   - sentence building with modal verbs learned so far,
   - every new word or phrase added for the current lesson.
2. Write the source text for all the exercise types listed above in Russian so the user practises translating into Dutch.
3. Where meaningful, include plural nouns and a mixture of `de`-words and `het`-words in those exercises.
4. Give each standard exercise 15-20 sentences/items. The current-lesson vocabulary exercise may contain as many items as needed to cover every new word and phrase.
5. Keep the existing Russian-to-Dutch and English-to-Dutch translation sections as separate sections.
6. Keep the dedicated plural and `de`/`het` exercises.
7. Include one dedicated exercise that collectively covers all new vocabulary introduced in the current lesson.
8. Provide a fixed answer key for every item; do not use open-ended tasks.
9. In conjunction and modal-verb exercises, do not name the required conjunction or modal verb beside each sentence. The user should choose it independently. The answer key may show one natural solution even when other correct variants are possible.

## Style

- Be clear, practical, and beginner-friendly.
- Use Dutch examples with English or Russian support when helpful.
- Do not over-explain advanced grammar unless needed.
- Make exercises easy to print or copy into notes.
- Keep answer keys separated from exercises.
