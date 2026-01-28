# Contributing to Plain English Book of Mormon Translations

Thank you for your interest in improving the Plain English Book of Mormon translations!

## How to Contribute

### Reporting Issues

If you find a translation error, awkward phrasing, or have a suggestion:

1. [Open an issue](https://github.com/plainenglishbom/plainenglishbom-translations/issues/new)
2. Include the book, chapter, and verse number
3. Quote the current translation
4. Suggest your improvement and explain why

### Submitting Changes

1. Fork this repository
2. Create a branch for your changes (`git checkout -b fix/1-nephi-3-7`)
3. Make your edits to the JSON files
4. Commit with a clear message (e.g., "Fix 1 Nephi 3:7 - clarify phrasing")
5. Open a Pull Request

## Translation Guidelines

When suggesting changes, please keep these principles in mind:

### Do

- Use clear, modern English that's easy to understand
- Preserve the original meaning and doctrinal content
- Keep verse boundaries intact
- Use natural sentence flow

### Don't

- Add interpretation or commentary
- Change doctrinal meaning
- Merge or split verses
- Use slang or overly casual language

## JSON Format

Each verse has this structure:

```json
{
  "number": 7,
  "text": "I, Nephi, said to my father..."
}
```

- `number` - Verse number (do not change)
- `text` - The translation (this is what you can improve)

To reference the original King James text, visit [plainenglishbom.com](https://plainenglishbom.com) or any standard Book of Mormon.

## Questions?

Open an issue with the "question" label or reach out at [plainenglishbom.com](https://plainenglishbom.com).
