---
name: markdown-editor
description: Use this when asked to edit, normalize, standardize, or improve Markdown files in this repository, especially after changes to .md or .mdx files.
---

# Markdown house-style editor (Part 2)

## Purpose

Apply WiseTech Academy Part 2 grammar and style rules to Markdown files.

This skill must:

- edit Markdown directly
- preserve factual information, domain terms, and technical intent
- default to U.S. English unless the user explicitly requests Australian English

## When to use

Use this skill when the user asks to:

- edit style, grammar, or syntax in a Markdown file
- normalize Markdown to house style
- proofread and standardize headings, lists, punctuation, spelling, and terminology presentation

Do not use this skill for:

- rewriting factual claims
- changing technical meaning
- authoring net-new long-form content from scratch unless explicitly requested

## Non-negotiable guardrails

Never change or reinterpret:

- factual statements, legal meaning, and compliance intent
- names, numbers, dates, percentages, currencies, standards, references, and URLs
- domain terms and product/brand names unless correcting casing to approved house form

Always preserve:

- code fences, inline code, links, and citation targets
- quote boundaries and attribution
- list hierarchy meaning (even if style is normalized)

If a change could alter meaning, choose minimal-change editing and keep source semantics.

## Rule precedence

Apply rules in this order:

1. Meaning and factual preservation
2. Legal, brand, trademark, and naming correctness
3. Language variant rule (U.S. English by default)
4. Markdown validity and structural integrity
5. Style and readability polish

## Workflow

1. Scan file and classify sections: headings, body text, lists, callouts, quotes, links, references.
2. Detect style violations against rules below.
3. Rewrite in place with minimal semantic movement.
4. Validate Markdown structure: headings, list continuity, blockquotes, code fences, links.
5. Run a safety pass: verify no factual drift and no term drift.
6. Final pass for consistency (spelling variant, punctuation, list style, heading style).

## Core editing rules

### Abbreviations and acronyms

- Avoid excessive abbreviations.
- At first occurrence on a page/section, write the term in full with acronym in parentheses.
- Use acronym alone on later occurrences.
- Keep common Latin abbreviations punctuated: e.g., i.e., etc.
- Title abbreviations typically do not use periods: Mr, Dr, Prof.

### Contractions and pronouns

- Do not use contractions in course prose.
- Allow contractions only if user explicitly says transcript/dialogue tone.
- Replace gendered generic pronouns with neutral forms: they/their.

### Ampersand

- Use "and" instead of "&".
- Exception: official names or UI labels that intentionally use "&".

### Apostrophes

- Use apostrophes for contractions and possession.
- Do not use apostrophes for plurals of acronyms, years, or numbers.

### Brand and terminology presentation

- Keep approved forms: WiseTech Global, WiseTech Academy.
- Disallow incorrect forms: Wise Tech, Wise-Tech, Wisetech.
- First-use acronym expansion applies to WTG and WTA.
- Use COVID-19 exactly; allow post-COVID-19.
- Use Incoterms® with registered symbol.

### Spelling and language variant

- Use U.S. English spelling by default.
- Switch to Australian spelling only if user explicitly requests AU audience.

### Capitalization and headings

- Use sentence case for headings/subheadings.
- Capitalize proper nouns, official titles, acronyms, and approved field/module names.
- Avoid terminal punctuation in headings where possible.
- In assessment text, emphasize NOT with capitals only; do not add bold.

### Colons, semicolons, and punctuation spacing

- Use colons to introduce lists or expansions.
- No space before punctuation; single space after sentence-ending punctuation.
- Use semicolons sparingly; prefer sentence split or comma where clearer.
- Use Oxford commas.
- No spaces around slashes in inline text.
- Do not use underlining.

### Dashes

- Hyphen for compound words (for example, step-by-step).
- En dash for ranges and contrast pairs (for example, 1914–18 and Paris–Dakar).
- For parenthetical breaks, prefer rewriting into shorter sentences; if used, keep spaces around en dash.

### Dates, times, numbers, currencies, units

- Acceptable date forms:
  - 8 July 1980
  - 24/06/2023
- Use numerals for decades and centuries as appropriate: 1960s, 21st century.
- Use 12-hour time format with hard-up am/pm (for example, 5pm).
- Write numbers one to nine as words, and 10+ as numerals, except technical/statistical contexts.
- Use U.S. numeric formatting: comma thousands, point decimals.
- Keep no space before % sign.
- Use currency code plus space before amount: AUD 100,000; USD 1.01; EUR 150.
- Do not replace currency codes with symbols and do not convert currencies.
- Use a space between number and unit: 10 cm, 30 m, 10 kg.

### Lists

- Always provide a lead-in sentence ending with a colon before a list.
- Keep list style consistent within a list level.
- Do not mix sentence fragments with full-sentence items in one list.
- Default list fragments: lowercase start, no terminal period.
- Full-sentence list items: sentence case and terminal period.
- Use numbered lists for steps/sequences and format as:
  1.  Item one.
  2.  Item two.
  3.  Item three.
- Prefer no deeper than three list levels unless source legal structure requires deeper nesting.

### Callout boxes in Markdown

- Convert callout categories to blockquote form with bold heading label on first line.
- Format:

> **Take note**
> Content for note text.

> **Example**
> Content for example text.

- Allowed labels include: Take note, Example, Case Study, Quote, Danger zone, Did you know, Helpful hints/tips, Alert, Exercise.
- Keep label capitalization exactly as house style (for example, Case Study in title-style capitalization).

### Quotes and references

- Use double quotation marks for inline quotes and single marks for quote-within-quote.
- Keep punctuation placement consistent with quoted sentence boundaries.
- For longer quotes, keep source lead-in and clear source attribution.
- Preserve link title capitalization/punctuation from source websites.
- Do not rewrite quoted external thought in a way that introduces copyright risk.

### Legislation, standards, glossary conventions

- Italicize primary legislation (Acts) in body text, except when the Act appears in headings.
- Do not italicize lower legislation forms (Rules, Regulations, Orders) or jurisdictions.
- On first mention, use full Act title + year + short form in parentheses; use short form later.
- Use "in accordance with" for mandatory legal/standard references when phrasing required criteria.
- Capitalize "Standard" when referring to a formal Australian or International Standard.
- For glossary entries:
  - use lowercase terms unless proper noun/acronym
  - do not repeat the term at the start of its definition
  - use U.S. spelling in glossary definitions by default

## Markdown integrity checks

Before finalizing, confirm:

- heading levels remain coherent
- list indentation and numbering render correctly
- blockquotes and callout labels render correctly
- code fences are balanced and unchanged unless formatting correction is required
- links are valid and unchanged unless explicitly requested

## Acceptance checklist

All must be true:

- markdown is valid and readable
- no factual or domain-term drift
- house style rules are consistently applied
- U.S. English is used unless AU was explicitly requested
- callouts are rendered as blockquotes with bold labels
- edits are direct and minimal-change where ambiguity exists

## Ambiguity handling

If rules conflict or context is incomplete:

- apply precedence order
- choose minimal-change edits
- preserve source meaning over stylistic strictness
- keep unresolved interpretation neutral and non-destructive
