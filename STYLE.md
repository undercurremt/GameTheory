# Lesson style guide (Curriculum v2.0)

Every lesson follows this shape. Reference lesson: `part-02/lesson_017_nash_equilibrium.md`.

## Skeleton

```markdown
# Lesson NNN — English Title

**Основна концепция:** …  
**Предпоставки:** Lessons NNN — Title, …        (omit if none)  
**Напречни връзки:** Lessons NNN, NNN           (omit if none)

---

> **Водещ въпрос:** …?

Intro paragraph: what we know from the previous lesson, what this one adds.

## 1. … (intuition through a concrete example)
## 2. … (method / mechanism)
## 3. … (formula, only after the intuition, every symbol explained)
## N. Какво … не казва / Какво да не бъркаме   (short list, only real pitfalls)
## N+1. Провери се                              (4–6 questions, answers in <details>)

## Накратко      (2–4 sentences that answer the guiding question)

**Следва:** Lesson NNN — Title. One-sentence teaser.

---

## Източници
```

## Rules

- **Fewer headings.** 6–9 `##` sections; `###` only when a section has two clearly separate parts. Prose, not fragments.
- **Order: example → intuition → formula.** Open with a running example (named people: Ана, Борис, …) and reuse it later in the lesson.
- **Math:** main text uses the simplest form (two players, explained symbols). General/heavy notation goes into
  `<details><summary><b>За желаещите:</b> …</summary> … </details>` with blank lines inside the block.
- **Caveats once.** No per-lesson "Стандарт на четене" block or status footer — the reading note lives on the homepage.
  Say what a concept does *not* imply once, in its own short section.
- **Headings in Bulgarian**; an English term is given once in parentheses where it is introduced, e.g. „доминиране (dominance)“.
- **Answers hidden** in `<details>`; questions in `<summary>`.
- **Cross-references** use v2.0 numbers from `curriculum.yaml`; the header lines mirror its prerequisites/related.
- **Sources:** primary works and standard textbooks; full bibliographic data, DOI where it exists.
- Length: roughly 1,000–1,800 words.
