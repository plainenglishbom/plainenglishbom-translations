# Plain English Book of Mormon Translations

This repository contains the plain English translations of the Book of Mormon, created by [The Plain English Book of Mormon Project](https://plainenglishbom.com).

## About

This translation aims to make the Book of Mormon accessible to modern readers by converting archaic King James English into clear, contemporary language. "Thee," "thou," "hath," "wherefore," and complex sentence structures are updated while preserving the meaning and message.

## Available Languages

- **English** (`en/`) - Modern English translation from King James English
- **Spanish** (`es/`) - Spanish translation

## Installation

```bash
# npm
npm install github:plainenglishbom/plainenglishbom-translations

# pnpm
pnpm add github:plainenglishbom/plainenglishbom-translations

# yarn
yarn add github:plainenglishbom/plainenglishbom-translations
```

## Usage

```javascript
const { en, es } = require('@plainenglishbom/translations');

// Access a verse
const verse = en.books[0].chapters[0].verses[0];
console.log(verse.plainText); // Modern English translation
console.log(verse.text);      // Original King James text
```

```typescript
import { en, es, BookOfMormon } from '@plainenglishbom/translations';

// TypeScript support included
const nephi: Book = en.books[0];
```

## Data Structure

```typescript
interface BookOfMormon {
  title: string;
  books: Book[];
}

interface Book {
  name: string;       // e.g., "The First Book of Nephi"
  shortName: string;  // e.g., "1 Nephi"
  chapters: Chapter[];
}

interface Chapter {
  number: number;
  verses: Verse[];
}

interface Verse {
  number: number;
  text: string;       // Original King James text
  plainText?: string; // Plain English translation
}
```

## Contributing

We welcome contributions to improve the translations! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## License

This work is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

The underlying text of the Book of Mormon is in the public domain. This license applies to the translation work.

## Links

- Website: [plainenglishbom.com](https://plainenglishbom.com)
- Report Issues: [GitHub Issues](https://github.com/plainenglishbom/plainenglishbom-translations/issues)
