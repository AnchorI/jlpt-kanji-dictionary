# JLPT Kanji Dictionary

A structured and enriched dataset for Japanese language learners and developers. This repository provides comprehensive information about Japanese **kanji characters** and **vocabulary words** used across **JLPT levels N5 to N1**.

---

## 📂 Contents

### 1. `jlpt-kanji.json`

A list of kanji used in JLPT exams, including:

- `kanji`: The character itself.
- `strokes`: Number of strokes to write the kanji.
- `radical_number`: The index of the kanji's radical.
- `frequency`: Kanji frequency rank (lower = more common).
- `jlpt`: JLPT level (`N5` to `N1`).
- `begins`: Number of words where this kanji appears at the beginning.
- `used_in`: Total number of words containing this kanji.
- `component_in`: Number of kanji that this kanji helps compose.
- `description`: A brief English explanation.

### 2. `dictionary.json`

A list of Japanese words, including:

- `kanji`: Word in kanji.
- `reading`: Reading in kana (hiragana).
- `pos`: Part of speech (abbreviated, see `dictionary-tags.json`).
- `glossary_en`: English definitions and example sentences.
- `glossary_ru`: Russian translations (optional).
- `sequence`: Usage frequency (higher = more frequent; negative = rare).

### 3. `dictionary-tags.json`

A decoding file for part-of-speech (POS) abbreviations used in `dictionary.json`.

---

## 🧩 Use Cases

- Language learning apps
- Linguistic research
- JLPT preparation tools
- Kanji/vocabulary search engines
- Educational games
- Import into Elasticsearch, SQLite, or other databases

---

## 🔧 Example

```json
{
  "kanji": "加担",
  "reading": "かたん",
  "pos": "n vs vi",
  "glossary_en": [
    "support",
    "participation",
    "assistance",
    "complicity",
    "conspiracy"
  ],
  "glossary_ru": [
    "1) помощь; поддержка; участие (в чём-л.)",
    "2) сговор; соучастие"
  ],
  "sequence": 1590450
}

