# Contributor Style Guide

This guide establishes formatting rules for transcriptions in the "Voices of the Congress" archive. Consistency ensures that all documents are readable, searchable, and maintain historical accuracy.

## General Principles

1. **Faithfulness**: Transcribe the text exactly as it appears in the source document. Do not modernize spelling, grammar, or punctuation unless the original is clearly a typographical error (in which case note the correction in a footnote).
2. **Clarity**: Use markdown formatting to improve readability while preserving the original structure.
3. **Transparency**: Clearly indicate any editorial interventions (unclear words, conjectures, omissions) using the conventions below.

## File Format

- All transcriptions are stored as Markdown (`.md`) files in the `transcriptions/` directory.
- Name files using the pattern `speaker_year_description.md` (e.g., `goldmann_1946_opening_address.md`).
- Start each file with a YAML front matter (optional) that includes metadata:
  ```yaml
  ---
  speaker: Nahum Goldmann
  date: 1946-08-XX
  source: goldmann_1946_speech.pdf
  language: English
  ---
  ```

## Text Formatting

### Speaker Identification
- When a speech begins, indicate the speaker on a separate line preceded by `**Speaker**:`  
  Example: `**Speaker**: Nahum Goldmann`

- If the document contains multiple speakers (e.g., a debate), introduce each new speaker with `**Speaker**: [Name]`.

### Paragraphs and Line Breaks
- Preserve the paragraph breaks of the original.
- Use a blank line between paragraphs (standard Markdown).

### Unclear or Illegible Words
- If a word or phrase cannot be read with certainty, enclose your best guess in square brackets and precede it with a question mark: `[? unclear word]`.
- If the text is completely missing or indecipherable, use `[illegible]` or `[gap]`.

### Editorial Notes
- Add explanatory notes in footnotes. Place a footnote marker `[^1]` in the text and define the note at the bottom of the document.
- Example: `The situation in Palestine[^1] was…`  
  At the bottom: `[^1]: Refers to the British Mandate period.`

### Foreign Terms and Transliteration
- Foreign words that are not commonly used in English should be italicized and followed by a translation in parentheses: `*aliyah* (immigration to Palestine)`.
- For Hebrew, Yiddish, or other languages written in non‑Latin scripts, provide a transliteration following the scholarly conventions of the Library of Congress.

### Headings and Document Structure
- Use Markdown headings (`#`, `##`, etc.) to reflect the document’s internal sections (e.g., `# Opening Remarks`, `## Discussion`).

## Validation

- Before submitting a pull request, proofread your transcription against the source document at least twice.
- If possible, have another contributor spot‑check a random sample of the text.

## Questions?

If you encounter a formatting dilemma not covered here, open an issue in the repository and tag it with `question` and `style-guide`. The maintainers will update this guide accordingly.

Thank you for helping preserve these important historical voices!