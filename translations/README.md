# Translation Files

This directory contains Quran translation files in JSON format.

## File Format

Each translation file should follow this structure:

```json
{
  "metadata": {
    "name": "Translation Name",
    "language": "language_code",
    "language_name": "Language Display Name",
    "translator": "Translator Name",
    "description": "Brief description",
    "version": 1,
    "total_verses": 6236,
    "created_at": "ISO 8601 timestamp"
  },
  "data": [
    {
      "surah": 1,
      "ayah": 1,
      "text": "Translation text for this verse"
    }
  ]
}
```

## Fields Description

### Metadata

- `name`: Official name of the translation
- `language`: ISO 639-1 language code (e.g., "en", "bn", "ar")
- `language_name`: Display name of the language
- `translator`: Name of the translator or translation organization
- `description`: Brief description of the translation
- `version`: Version number of the translation
- `total_verses`: Total number of verses (should be 6236)
- `created_at`: ISO 8601 timestamp of when the file was created

### Data Array

Each object in the data array represents one verse:

- `surah`: Surah number (1-114)
- `ayah`: Ayah number within the surah
- `text`: The translated text of the verse

## Available Translations

### Bundled (Included in App)

- `en.sahih.json` - Sahih International (English)
- `bn.taisirul.json` - Taisirul Quran (Bengali) - TODO

### Downloadable

- `ur.maududi.json` - Mufti Taqi Usmani (Urdu) - TODO
- `ar.jalalayn.json` - Tafsir Al-Jalalayn (Arabic) - TODO
- `hi.hindi.json` - Hindi Translation - TODO
- `id.indonesian.json` - Indonesian Translation - TODO
- `tr.turkish.json` - Turkish Translation - TODO
- `fr.hamidullah.json` - Muhammad Hamidullah (French) - TODO
- `de.bubenheim.json` - Abu Rida (German) - TODO
- `es.cortes.json` - Raúl González Bórnez (Spanish) - TODO

## Adding a New Translation

1. Create a new JSON file following the format above
2. Ensure all 6236 verses are included
3. Update `lib/core/database/seeds/data/translation_seed.dart` to include the new translation metadata
4. Add the download URL or bundle the file with the app

## Verse Count by Surah

Total verses: 6236

| Surah | Name       | Verses |
| ----- | ---------- | ------ |
| 1     | Al-Fatihah | 7      |
| 2     | Al-Baqarah | 286    |
| 3     | Ali 'Imran | 200    |
| 4     | An-Nisa    | 176    |
| 5     | Al-Ma'idah | 120    |
| ...   | ...        | ...    |
| 114   | An-Nas     | 6      |

## Notes

- The `en.sahih.json` file currently contains only sample verses from Surah 1 and the beginning of Surah 2
- You need to complete the file with all 6236 verses
- Ensure proper JSON formatting and UTF-8 encoding
- Test the file before deploying to ensure it loads correctly
