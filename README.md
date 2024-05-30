# Quran Text

## Summary

| Filename | Format | Description |
|----------|--------|-------------|
| `quran-flat-no-tashkeel.txt` | Text | Whole Quran in single line with no tashkeel. |
| `quran-flat-min-tashkeel.txt` | Text | Whole Quran in single line with minimal tashkeel. |
| `quran-flat-full-tashkeel.txt` | Text | Whole Quran in single line with full tashkeel. |
| `quran-no-tashkeel.json` | Text | JSON format with no tashkeel<sup>*</sup> |
| `quran-min-tashkeel.json` | Text | JSON format with minimal tashkeel<sup>*</sup> |
| `quran-full-tashkeel.json` | Text | JSON format with full tashkeel<sup>*</sup> |

<sup>*</sup> The JSON format is array of surahs, each object in array contains following properties:

```json
{
  "id": 1,
  "name": "الفاتحة",
  "transliteration": "Al-Fatihah",
  "type": "meccan",
  "total_verses": 7,
  "verses": [ ... ]
}
```

The `id` is surah number

each `verse` contains following properties

```json
{
  "id": 1,
  "text": "بِسۡمِ ٱللَّهِ ٱلرَّحۡمَٰنِ ٱلرَّحِيمِ"
}
```

the `id` is verse number
