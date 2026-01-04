# Dasanama

![Data Format: JSON](https://img.shields.io/badge/Format-JSON-orange.svg)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**Dasanama** is a specialized synonym mapping dataset designed to enhance search relevancy for Japanese names, entities, and terminology. It provides a standardized bridge between Kanji characters and their various Romaji transliterations to ensure high-quality search recall.

---

## Purpose & Scope

This dataset addresses common challenges in Japanese text retrieval:

1. **Kanji-to-Romaji Mapping**: Providing phonetic readings for Kanji names that search systems may not natively resolve (e.g., `早見` → `hayami`, `裕貴` → `yuki`).
2. **Transliteration Standardization**: Handling variations in Romaji spelling, especially regarding long vowels and common naming conventions:
    * **Long Vowels**: Mapping `yuki` to `yuuki`, `ohta` to `oota`, or `soma` to `souma`.
    * **Name Variants**: Ensuring that different Romanization styles point to the same phonetic identity.

---

## Repository Structure

* [synonyms.json](synonyms.json): The consolidated mapping file. Each key represents a search term (Kanji or Romaji), and the value is an array of its corresponding synonyms or readings.

---

## Integration

The data is provided in a standard JSON format, making it compatible with most modern search engines, databases, and custom applications.

### Example Data Format

```json
{
    "早見": ["hayami"],
    "裕貴": ["yuki", "yuuki"],
    "ito": ["itou"],
    "ohta": ["oota"]
}
```

---

## License

[MIT](/LICENSE)
